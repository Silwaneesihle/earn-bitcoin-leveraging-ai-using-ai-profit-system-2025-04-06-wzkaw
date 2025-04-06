# AI Profit System Landing Page - Maintenance Guide

This guide will help you maintain and customize the AI Profit System landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Header Section
The header contains the logo and main navigation button:

```html
<header class="fixed w-full bg-white/95 backdrop-blur-sm z-50 border-b border-gray-100">
    <!-- Logo Text -->
    <div class="text-2xl font-bold bg-gradient-to-r from-blue-600 to-indigo-600 bg-clip-text text-transparent">
        AI Profit System
    </div>
```

To modify:
1. Change logo text: Replace "AI Profit System" with your desired text
2. Adjust logo size: Modify `text-2xl` to `text-3xl` for larger or `text-xl` for smaller
3. Change colors: Update `from-blue-600 to-indigo-600` with different Tailwind color classes

### Hero Section
The main banner section includes:

```html
<h1 class="text-4xl md:text-6xl font-bold text-white leading-tight mb-6">
    Earn Bitcoin Leveraging AI using AI Profit System
</h1>
<p class="text-xl md:text-2xl text-gray-200 mb-8">
    24/7 AI Assistant, No KYC, Increased Profits
</p>
```

To modify:
1. Update heading: Replace the h1 text content
2. Change subtitle: Modify the paragraph text
3. Adjust responsive text sizes:
   - `text-4xl md:text-6xl`: Mobile and desktop sizes
   - `text-xl md:text-2xl`: Subtitle sizes

### Features Section
Each feature card follows this structure:

```html
<div class="bg-white p-8 rounded-2xl shadow-lg hover:shadow-xl transition duration-300">
    <!-- Icon container -->
    <div class="w-12 h-12 bg-blue-100 rounded-full flex items-center justify-center mb-6">
        <!-- SVG icon here -->
    </div>
    <h3 class="text-xl font-semibold mb-4">Decentralized</h3>
    <p class="text-gray-600">Fully decentralized system ensuring your privacy...</p>
</div>
```

To modify:
1. Change feature title: Update the h3 text
2. Modify description: Update the paragraph text
3. Adjust spacing: Modify `p-8` padding or `mb-6` margin values
4. Change hover effects: Modify `hover:shadow-xl` class

## Fixing Broken Links

### Current Link Locations

1. Navigation Button:
```html
<a href="https://go.e1ulife.com/ai-takeover?affid=Silwane1" class="text-white">Get Started</a>
```

2. Hero CTA Button:
```html
<a href="https://go.e1ulife.com/ai-takeover?affid=Silwane1" class="inline-block px-8 py-4...">
```

To update links:
1. Locate the `href` attribute
2. Replace the URL with your new destination
3. Ensure the `class` attributes remain unchanged
4. Test the link after updating

Example:
```html
<a href="https://your-new-link.com" class="text-white">Get Started</a>
```

## Linking Privacy and Terms Pages

The footer contains placeholder links for Privacy Policy and Terms of Service:

```html
<div>
    <h3 class="text-white font-semibold mb-4">Legal</h3>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To add proper links:
1. Create your privacy.html and terms.html files
2. Update the href attributes:

```html
<li><a href="privacy.html" class="hover:text-white transition duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition duration-300">Terms of Service</a></li>
```

## Troubleshooting

Common issues and solutions:

1. **Broken Responsive Design**
   - Check for `md:` and `lg:` prefixes in classes
   - Ensure viewport meta tag is present
   - Test on different screen sizes

2. **Missing Styles**
   - Verify Tailwind CDN link is working
   - Check for typos in class names
   - Ensure classes are properly spaced

3. **Link Issues**
   - Test all links after updating
   - Use relative paths for internal pages
   - Verify external URLs are correct and accessible

Remember to:
- Always backup before making changes
- Test on multiple browsers
- Validate HTML using W3C validator
- Check mobile responsiveness
- Keep consistent styling throughout

For additional help, refer to:
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [HTML MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/HTML)