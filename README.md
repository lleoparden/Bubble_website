# Bubble Chat App Website

This repository contains a simple, responsive website for the Bubble chat application. The website includes a home page, download page, terms of service, and privacy policy.

## Table of Contents

1. [Features](#features)
2. [File Structure](#file-structure)
3. [Setup Instructions](#setup-instructions)
4. [Customization](#customization)
5. [Deployment](#deployment)
6. [Troubleshooting](#troubleshooting)
7. [Contributing](#contributing)
8. [License](#license)

## Features

- **Responsive Design**: Works on mobile, tablet, and desktop devices
- **Light/Dark Mode**: Toggle between light and dark themes
- **Single-Page Application**: Navigation occurs without page reloads
- **Download Page**: APK download functionality
- **Legal Pages**: Terms of Service and Privacy Policy included
- **Modern UI**: Clean, attractive interface using Bubble's color scheme

## File Structure

```
bubble-website/
├── index.html              # Main HTML file containing all code
├── bubble_app.apk          # Your application APK file
├── README.md               # This README file
└── assets/                 # Optional folder for any additional assets
    └── favicon.ico         # Website favicon (optional)
```

## Setup Instructions

1. **Clone or download this repository**

2. **Place your APK file in the root directory**
   - Rename your APK to `bubble_app.apk` or update the download link in the HTML file

3. **Test locally**
   - Open `index.html` in a web browser to preview the site
   - Note: The download functionality may not work fully in local testing

## Customization

### Updating Content

The website is contained in a single HTML file with inline CSS and JavaScript. To modify content:

1. **General Information**
   - Update app descriptions in the home page sections
   - Modify feature descriptions in the "Why Choose Bubble?" section
   - Change the version information in the download page

2. **Legal Documents**
   - Review and update the Terms of Service and Privacy Policy to match your app's specific features and data handling practices
   - Update the contact email addresses and effective dates

3. **APK File**
   - Replace `bubble_app.apk` with your actual APK file
   - Update version number, size, and requirements in the download section

### Styling and Colors

All styling is contained in the `<style>` section at the top of the HTML file. The color scheme uses CSS variables defined in the `:root` selector:

```css
:root {
    --primary-color: #9BA8DD;
    --secondary-color: #665695;
    --bg-color: #F2F2FF;
    --text-color: #665695;
    --button-color: #9BA8DD;
    --button-hover: #ABB5E8;
    --header-bg: #D2D2EF;
}
```

For dark mode, these variables are redefined in the `body.dark-mode` selector.

### Adding Images

To add real images:

1. Create an `images` folder in your project directory
2. Add your images to this folder
3. Replace placeholder image references like:
   ```html
   <img src="/api/placeholder/400/320" alt="Bubble App Interface" />
   ```
   with your actual images:
   ```html
   <img src="images/app-screenshot.png" alt="Bubble App Interface" />
   ```

## Deployment

### Basic Web Hosting

1. **Purchase a domain name** (e.g., `bubblechatapp.com`)
2. **Choose a web hosting provider** (e.g., Netlify, Vercel, GitHub Pages, AWS S3)
3. **Upload the files** to your hosting provider
   - Make sure to include `index.html` and `bubble_app.apk`
4. **Configure your domain** to point to your hosting provider

### Using GitHub Pages (Free Option)

1. Create a GitHub repository
2. Upload your website files to the repository
3. Go to Settings > Pages
4. Set the source to your main branch
5. Your site will be available at `https://yourusername.github.io/repository-name/`

## Troubleshooting

### APK Download Issues

If users have trouble downloading the APK:

1. Make sure the MIME types are correctly configured on your server
2. For Apache servers, add this to your `.htaccess` file:
   ```
   AddType application/vnd.android.package-archive apk
   ```
3. Consider providing alternative download links or QR codes

### Display Issues

If the website doesn't display correctly:

1. Make sure you're using a modern browser
2. Check for JavaScript errors in the browser console
3. Verify that all files are uploaded correctly

## Contributing

If you'd like to contribute to the development of this website:

1. Fork the repository
2. Create a new branch for your feature
3. Make your changes
4. Submit a pull request

## License

[Your chosen license here]

---

*This website was created for the Bubble Chat Application. © 2025 Bubble Chat App. All rights reserved.*
