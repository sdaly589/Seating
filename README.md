# Christmas Party Seating Finder

A simple web app to help guests find their table number at your office Christmas party.

## Setup Instructions

### 1. Publish Your Google Sheet as CSV

1. Open your Google Sheet: https://docs.google.com/spreadsheets/d/1Kz0yIlmMH5FqoRiEyEZs8_kweNFtRFMkPLMpMDjlYc8/edit
2. Go to **File** → **Share** → **Publish to web**
3. In the dropdown, select your sheet and choose **Comma-separated values (.csv)**
4. Click **Publish**
5. Copy the URL (it will look like: `https://docs.google.com/spreadsheets/d/e/2PACX-.../pub?output=csv`)

### 2. Update the HTML File

1. Open `index.html`
2. Find the line: `const CSV_URL = 'YOUR_PUBLISHED_CSV_URL_HERE';`
3. Replace `YOUR_PUBLISHED_CSV_URL_HERE` with your published CSV URL

### 3. Enable GitHub Pages

1. Push this repository to GitHub
2. Go to your repository settings
3. Navigate to **Pages** (in the left sidebar)
4. Under **Source**, select **main** branch
5. Click **Save**
6. Your site will be available at: `https://sdaly589.github.io/Seating/`

### 4. Generate QR Code

Once your site is live, use any free QR code generator:
- [QR Code Generator](https://www.qr-code-generator.com/)
- [QRCode Monkey](https://www.qrcode-monkey.com/)

Enter your GitHub Pages URL and download the QR code!

## How It Works

- Guests scan the QR code at the front door
- They type their name in the search box
- The app shows their table number in large, clear text
- No login or authentication required!

## Google Sheet Format

Make sure your Google Sheet has these columns:
- A column with "Name" (guest names)
- A column with "Table" (table numbers)

The script will automatically detect these columns.
