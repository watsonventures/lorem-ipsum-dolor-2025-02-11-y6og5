# Landing Page Maintenance Guide

This guide will help you maintain and customize your landing page. Follow these instructions carefully to make updates while preserving the design and functionality.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<!-- Original -->
<a href="#" class="text-2xl font-['Playfair_Display'] font-bold text-gray-900">Logo</a>

<!-- How to update -->
<a href="#" class="text-2xl font-['Playfair_Display'] font-bold text-gray-900">Your Company Name</a>
```

#### Hero Section
Look for the following sections to update main content:
```html
<h1 class="font-['Playfair_Display'] text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight mb-8">
    Lorem ipsum dolor
</h1>
```
Replace "Lorem ipsum dolor" with your headline text.

### Tailwind CSS Classes Explained

Key classes used in this landing page:

1. Layout Classes:
   - `max-w-7xl`: Maximum width container
   - `mx-auto`: Center content horizontally
   - `px-4`: Horizontal padding
   - `py-24`: Vertical padding

2. Responsive Design:
   - `md:text-5xl`: Applies font size on medium screens
   - `lg:text-6xl`: Applies font size on large screens

To modify spacing, use these patterns:
- Padding: `p-{number}` (e.g., `p-4`, `p-8`)
- Margin: `m-{number}` (e.g., `m-4`, `m-8`)
- Sizes increase in increments of 4 pixels

## Fixing Broken Links

### Navigation Menu Links
Current navigation links:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#contact">Contact</a>
</div>
```

To update:
1. Replace `#features` with your features section ID
2. Replace `#benefits` with your benefits section ID
3. Replace `#contact` with your contact section ID

### Call-to-Action Links
Look for:
```html
<a href="Lorem ipsum dolor" class="inline-flex items-center...">
```
Replace `"Lorem ipsum dolor"` with your actual URL.

## Adding Privacy and Terms Pages

### Footer Modification
Add privacy and terms links in the footer's "Links" section:

```html
<div>
    <h4 class="text-lg font-semibold text-white mb-4">Links</h4>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Features</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Benefits</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Contact</a></li>
        <!-- Add these new lines -->
        <li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

## Troubleshooting

### Common Issues and Solutions

1. Broken Layout
   - Check for missing closing tags
   - Verify Tailwind CSS classes are spelled correctly
   - Ensure proper nesting of div elements

2. Responsive Design Issues
   - Verify media query classes (md:, lg:) are properly placed
   - Test on different screen sizes using browser developer tools

3. Link Problems
   - Ensure all href attributes have valid values
   - Check that section IDs match their corresponding links
   - Verify file paths for privacy.html and terms.html

### Best Practices

1. Always maintain the responsive design structure:
   ```html
   <div class="text-base md:text-lg lg:text-xl">
   ```

2. Keep consistent spacing throughout sections:
   ```html
   <section class="py-24">
   ```

3. Preserve the gradient backgrounds:
   ```html
   <section class="bg-gradient-to-r from-purple-600 to-indigo-600">
   ```

Need additional help? Contact your web development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).