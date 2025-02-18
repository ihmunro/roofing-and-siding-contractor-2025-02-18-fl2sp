# RoofPro Landing Page - Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the RoofPro contractor landing page. Whether you're new to web development or need a quick reference, you'll find step-by-step guidance for common updates.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your company name and navigation menu:
```html
<a href="#" class="text-2xl font-bold text-gray-900">RoofPro</a>
```
To change the company name:
1. Locate this line in the header section
2. Replace "RoofPro" with your company name
3. Adjust font size if needed by modifying `text-2xl` to `text-xl` (smaller) or `text-3xl` (larger)

### Hero Section
The main headline and subheading are located in:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 tracking-tight mb-6">
    Trusted Roofing and Siding Contractor
</h1>
<p class="text-xl text-gray-600 mb-8">
    Professional roofing and siding solutions for your home
</p>
```
To modify:
1. Replace the text between the `<h1>` tags for the main headline
2. Replace the text between the `<p>` tags for the subheading
3. Keep the existing classes to maintain responsive design

### Services Section
Each service card follows this structure:
```html
<div class="bg-gray-50 rounded-xl p-8 shadow-lg hover:shadow-xl transition-shadow duration-300">
    <h3 class="text-2xl font-semibold mb-4">Roofing Services</h3>
    <p class="text-gray-600 mb-6">Professional roofing solutions...</p>
</div>
```
To add or modify services:
1. Copy the entire `<div>` block for a new service
2. Update the heading and description text
3. Maintain the existing classes for consistent styling

## Managing Links

### Navigation Menu Links
Current navigation links are:
```html
<div class="hidden md:flex space-x-8">
    <a href="#services" class="text-gray-600 hover:text-gray-900 font-medium transition-colors duration-300">Services</a>
    <a href="#estimates" class="text-gray-600 hover:text-gray-900 font-medium transition-colors duration-300">Estimates</a>
    <a href="#faq" class="text-gray-600 hover:text-gray-900 font-medium transition-colors duration-300">FAQ</a>
    <a href="#contact" class="text-gray-600 hover:text-gray-900 font-medium transition-colors duration-300">Contact</a>
</div>
```
To update links:
1. For internal page sections, use `#section-id` format
2. For external pages, use full URLs (e.g., `https://example.com`)
3. For local pages, use relative paths (e.g., `about.html`)

### Social Media Links
Located in the footer:
```html
<div class="flex space-x-4 mt-4">
    <a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">
        <!-- Facebook icon -->
    </a>
</div>
```
To update:
1. Replace the `#` with your social media profile URLs
2. Test links to ensure they open in the correct location

## Adding Privacy and Terms Pages

### Footer Legal Links
Current placeholder links:
```html
<div>
    <h3 class="text-xl font-bold mb-4">Legal</h3>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```
To link privacy and terms pages:
1. Create `privacy.html` and `terms.html` in your root directory
2. Update the href attributes:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues

1. **Broken Links**
   - Check for typos in URLs
   - Verify file names match exactly
   - Ensure files are in the correct directory

2. **Styling Problems**
   - Don't remove `class` attributes
   - Maintain responsive classes (those starting with `md:` or `lg:`)
   - Keep transition classes for smooth animations

3. **Layout Issues**
   - Preserve container classes (`container mx-auto`)
   - Maintain grid classes (`grid grid-cols-1 md:grid-cols-2`)
   - Keep padding and margin classes (`p-8`, `mb-4`, etc.)

### Getting Help
- Check the [Tailwind CSS documentation](https://tailwindcss.com/docs) for styling references
- Validate HTML at [W3C Validator](https://validator.w3.org/)
- Test responsive design using browser developer tools

Remember to always test changes across different devices and browsers to ensure consistency.