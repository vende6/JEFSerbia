# JEF Serbia - Static Web App

A modern, responsive website for Young European Federalists Serbia, built as an Azure Static Web App.

## Features

- **Responsive Design**: Mobile-first approach with modern CSS Grid and Flexbox
- **Interactive Navigation**: Smooth scrolling and mobile hamburger menu
- **Contact Forms**: Join form and contact form with client-side validation
- **Modern UI**: Professional design with European blue color scheme
- **Animations**: Scroll-triggered animations and counter effects
- **SEO Optimized**: Semantic HTML structure and meta tags

## Structure

```
JEFSerbia/
├── index.html                 # Main HTML file
├── staticwebapp.config.json   # Azure Static Web Apps configuration
├── styles/
│   └── main.css              # Main stylesheet
├── scripts/
│   └── main.js               # JavaScript functionality
└── images/                   # Image assets (add your images here)
```

## Required Images

To complete the website, add these images to the `images/` folder:

- `jef-logo.png` - JEF Serbia logo (recommended: 200x80px)
- `hero-image.jpg` - Hero section image (recommended: 800x600px)
- `about-image.jpg` - About section image (recommended: 600x400px)
- `news-1.jpg`, `news-2.jpg`, `news-3.jpg` - News article images (recommended: 400x200px each)

## Local Development

1. Open the project folder in VS Code
2. Install the Live Server extension
3. Right-click on `index.html` and select "Open with Live Server"
4. The website will open in your browser at `http://localhost:5500`

## Deployment to Azure Static Web Apps

### Option 1: Using Azure Static Web Apps CLI

1. Install the CLI:
   ```bash
   npm install -g @azure/static-web-apps-cli
   ```

2. Initialize and deploy:
   ```bash
   swa init
   swa deploy --env production
   ```

### Option 2: Using GitHub Actions (Recommended)

1. Push your code to a GitHub repository
2. Create an Azure Static Web App in the Azure Portal
3. Connect it to your GitHub repository
4. Azure will automatically set up CI/CD with GitHub Actions

## Customization

### Colors
The main brand color is defined in CSS as `#1e3a8a` (European blue). You can change this throughout the CSS file.

### Content
- Update the content in `index.html` to match your organization's information
- Replace placeholder images with actual photos
- Update contact information and social media links

### Forms
The forms currently use client-side validation and show success messages. To make them functional:
- Set up a backend API or use Azure Functions
- Update the form submission handlers in `scripts/main.js`

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## License

This project is open source and available under the [MIT License](LICENSE).