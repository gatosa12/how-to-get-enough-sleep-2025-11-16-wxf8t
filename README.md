# Sleep Guide Landing Page - Maintenance & Customization Guide

A comprehensive guide for maintaining and customizing your "How to Get Enough Sleep" landing page. This document provides step-by-step instructions for beginners to update content, fix links, and customize the page without breaking functionality.

---

## Table of Contents

1. [Getting Started](#getting-started)
2. [Understanding the Page Structure](#understanding-the-page-structure)
3. [Updating Text Content](#updating-text-content)
4. [Modifying Tailwind CSS Classes](#modifying-tailwind-css-classes)
5. [Fixing and Managing Links](#fixing-and-managing-links)
6. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
7. [Common Customizations](#common-customizations)
8. [Troubleshooting](#troubleshooting)

---

## Getting Started

### What You Need

Before you begin editing this landing page, you'll need:

- **A text editor**: VS Code (recommended), Notepad++, or Sublime Text
- **Basic understanding**: HTML tags and what they do
- **File access**: The `index.html` file saved on your computer
- **A web browser**: To preview your changes (Chrome, Firefox, Safari, or Edge)

### How to Edit the File

1. **Open your text editor** (e.g., VS Code)
2. **Click File → Open** and select your `index.html` file
3. **Make your changes** using the instructions in this guide
4. **Save the file** using `Ctrl+S` (Windows) or `Cmd+S` (Mac)
5. **Preview changes**: Open the file in your browser by dragging it into a browser window or right-clicking and selecting "Open with Browser"

### Important Safety Tips

- **Always make a backup** of your original `index.html` before making changes
- **Make one change at a time** and test it before making another
- **Don't delete opening or closing tags** (like `<div>` and `</div>`)
- **Keep all quotes and brackets** intact when editing attributes

---

## Understanding the Page Structure

### Main Sections of Your Landing Page

Your landing page is organized into these major sections:

```
1. Header & Navigation (Fixed at top)
2. Hero Section (Large welcome area with call-to-action)
3. Features Section (Three main features: Exercise, Supplements, Bed)
4. Video Section (Embedded YouTube video)
5. Benefits Section (Three benefit areas with images)
6. About Us Section (Company story and mission)
7. Testimonials Section (Customer reviews)
8. FAQ Section (Frequently asked questions with expandable answers)
9. CTA Section (Call-to-action for contact)
10. Footer (Links and company info)
```

### How to Find Sections in Your Code

Each section starts with an HTML comment and an ID. For example:

```html
<!-- Features Section -->
<section id="features" class="py-24 bg-gray-900 relative">
```

To find a section quickly:
1. **Use Ctrl+F** (Windows) or **Cmd+F** (Mac) in your text editor
2. **Type the section name**, like `id="features"`
3. The editor will highlight and jump to that location

---

## Updating Text Content

### Hero Section - Main Headline

**Location**: Near the top of the page, after the hero section begins

**Current text**:
```html
<h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-bold text-white mb-6 leading-tight tracking-tight">
    How to Get Enough Sleep
</h1>
```

**How to change it**:

1. Find this section using `Ctrl+F` and searching for `How to Get Enough Sleep`
2. Replace the text between `>` and `</h1>` with your new headline
3. Example - to change it to "Sleep Better Tonight":
```html
<h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-bold text-white mb-6 leading-tight tracking-tight">
    Sleep Better Tonight
</h1>
```

**Important**: Keep all the `class="..."` information exactly as it is. Only change the text between the tags.

### Hero Section - Subheading

**Current text**:
```html
<p class="text-xl sm:text-2xl md:text-3xl text-gray-300 mb-8 leading-relaxed max-w-3xl mx-auto">
    Create Starting landing page in a minute
</p>
```

**How to change it**:

1. Search for `Create Starting landing page in a minute`
2. Replace with your new subheading
3. Example:
```html
<p class="text-xl sm:text-2xl md:text-3xl text-gray-300 mb-8 leading-relaxed max-w-3xl mx-auto">
    Improve Your Sleep in Just 7 Days
</p>
```

### Hero Section - Description Text

**Current text**:
```html
<p class="text-lg text-gray-400 mb-12 max-w-2xl mx-auto leading-relaxed">
    Discover proven strategies to improve your sleep quality and wake up refreshed every morning. Learn about the best exercises, supplements, and bedding solutions.
</p>
```

**How to change it**:

1. Search for `Discover proven strategies`
2. Replace the entire paragraph with your new description
3. Keep the `class="..."` exactly the same
4. Example:
```html
<p class="text-lg text-gray-400 mb-12 max-w-2xl mx-auto leading-relaxed">
    Transform your sleep tonight with our science-backed methods. Join thousands who've already improved their rest and energy levels.
</p>
```

### Features Section - Title and Description

**Location**: Search for `id="features"`

**Current Feature 1 title**:
```html
<h3 class="text-2xl font-bold text-white mb-4">Best Exercise</h3>
```

**How to change it**:

1. Search for `Best Exercise` (or find it in the features section)
2. Replace the text, keeping all HTML tags intact
3. Example:
```html
<h3 class="text-2xl font-bold text-white mb-4">Daily Movement & Exercise</h3>
```

**Current Feature 1 description**:
```html
<p class="text-gray-400 leading-relaxed mb-4">
    Regular physical activity is one of the most effective ways to improve sleep quality. Exercise helps regulate your circadian rhythm and reduces anxiety that can interfere with sleep.
</p>
```

**How to change it**:

1. Find the paragraph text starting with "Regular physical activity"
2. Replace it with your new description
3. Keep `class="text-gray-400 leading-relaxed mb-4"` exactly the same

**Repeat for Feature 2 and Feature 3**:
- Feature 2: Search for `Best Supplement`
- Feature 3: Search for `Best Comfortable Bed`

### Features Section - Bullet Points

**Current bullet points for Feature 1**:
```html
<ul class="space-y-2 text-gray-300">
    <li class="flex items-center">
        <i class="fas fa-check text-purple-400 mr-3"></i>
        <span>30 minutes daily activity</span>
    </li>
    <li class="flex items-center">
        <i class="fas fa-check text-purple-400 mr-3"></i>
        <span>Evening yoga for relaxation</span>
    </li>
    <li class="flex items-center">
        <i class="fas fa-check text-purple-400 mr-3"></i>
        <span>Avoid intense exercise before bed</span>
    </li>
</ul>
```

**How to change a bullet point**:

1. Find the text inside `<span>` tags, like `30 minutes daily activity`
2. Replace only the text between `<span>` and `</span>`
3. Example - to change the first bullet:
```html
<li class="flex items-center">
    <i class="fas fa-check text-purple-400 mr-3"></i>
    <span>Walk 10,000 steps daily</span>
</li>
```

**How to add a new bullet point**:

1. Copy an entire `<li>` block
2. Paste it right after the last `</li>` in that list
3. Change only the text in the `<span>` tag
4. Example:
```html
<li class="flex items-center">
    <i class="fas fa-check text-purple-400 mr-3"></i>
    <span>Your new bullet point here</span>
</li>
```

### Benefits Section - Titles and Content

**Location**: Search for `id="benefits"`

**Current Benefit 1 title**:
```html
<h3 class="text-3xl sm:text-4xl font-bold text-white mb-4 leading-tight">
    Sleep Like a Baby
</h3>
```

**How to change it**:

1. Search for `Sleep Like a Baby`
2. Replace with your new title
3. Example:
```html
<h3 class="text-3xl sm:text-4xl font-bold text-white mb-4 leading-tight">
    Deep, Restful Sleep Every Night
</h3>
```

**Current Benefit 1 description**:
```html
<p class="text-gray-400 text-lg leading-relaxed mb-6">
    Experience deep, uninterrupted sleep that leaves you feeling completely refreshed...
</p>
```

**How to change it**:

1. Find the paragraph text
2. Replace the entire text between `<p>` and `</p>`
3. Keep the `class="..."` exactly the same

**Repeat for Benefits 2 and 3**:
- Benefit 2: Search for `Wake Up Like a Champion`
- Benefit 3: Search for `Optimal Health & Wellness`

### Testimonials Section - Customer Reviews

**Location**: Search for `id="testimonials"`

**Current testimonial text**:
```html
<p class="text-gray-300 leading-relaxed mb-6 text-lg">
    "I was skeptical at first, but following the exercise recommendations and switching to a quality mattress changed everything..."
</p>
```

**How to change a testimonial**:

1. Find the testimonial you want to change
2. Replace the text between `<p>` and `</p>`
3. Keep the quotation marks at the beginning and end
4. Example:
```html
<p class="text-gray-300 leading-relaxed mb-6 text-lg">
    "This guide transformed my sleep in just two weeks. I'm more productive and energized than ever!"
</p>
```

**How to change the customer name**:

```html
<p class="text-white font-bold">Sarah Mitchell</p>
<p class="text-purple-400 text-sm">Business Executive, New York</p>
```

Replace `Sarah Mitchell` with the new name and update the title/location as needed.

### FAQ Section - Questions and Answers

**Location**: Search for `id="faq"`

**Current FAQ question**:
```html
<h3 class="text-lg font-bold text-white text-left">How long does it take to see improvements in my sleep?</h3>
```

**How to change a question**:

1. Find the question you want to change
2. Replace the text between `<h3>` and `</h3>`
3. Example:
```html
<h3 class="text-lg font-bold text-white text-left">What's the best time to exercise?</h3>
```

**Current FAQ answer**:
```html
<div class="accordion-content px-6 pb-4 text-gray-400">
    <p class="leading-relaxed">
        Most people notice improvements within 1-2 weeks...
    </p>
</div>
```

**How to change an answer**:

1. Find the answer text inside the `<p>` tag
2. Replace the entire paragraph with your new answer
3. Example:
```html
<div class="accordion-content px-6 pb-4 text-gray-400">
    <p class="leading-relaxed">
        The best time to exercise is 3-4 hours before bedtime. This gives your body time to cool down before sleep while still providing the sleep-promoting benefits of physical activity.
    </p>
</div>
```

### Footer Section - Company Information

**Location**: Search for `<footer>`

**Current company description**:
```html
<p class="text-gray-400 text-sm leading-relaxed mb-4">
    Dedicated to helping you achieve better sleep and transform your life through proven, science-backed methods.
</p>
```

**How to change it**:

1. Find this text in the footer
2. Replace it with your company description
3. Keep `class="text-gray-400 text-sm leading-relaxed mb-4"` the same

**Update copyright year**:

```html
&copy; 2024 Sleep Guide. All rights reserved.
```

Change `2024` to the current year and update company name if needed.

---

## Modifying Tailwind CSS Classes

### What Are Tailwind CSS Classes?

Tailwind CSS is a system of pre-made styling classes. Instead of writing custom CSS, you use class names to style elements. For example:

- `text-white` = white text color
- `bg-purple-600` = purple background
- `mb-6` = margin (space) below the element
- `rounded-lg` = slightly rounded corners

### Common Tailwind Classes Used in This Page

| Class | What It Does | Example |
|-------|-------------|---------|
| `text-white` | Makes text white | `<h1 class="text-white">` |
| `text-gray-300` | Makes text light gray | `<p class="text-gray-300">` |
| `bg-gray-900` | Dark gray background | `<div class="bg-gray-900">` |
| `bg-purple-600` | Purple background | `<button class="bg-purple-600">` |
| `px-8` | Horizontal padding (left & right) | `<div class="px-8">` |
| `py-4` | Vertical padding (top & bottom) | `<button class="py-4">` |
| `mb-6` | Margin below (space after) | `<p class="mb-6">` |
| `mt-4` | Margin top (space before) | `<h2 class="mt-4">` |
| `rounded-lg` | Slightly rounded corners | `<div class="rounded-lg">` |
| `shadow-lg` | Large drop shadow | `<div class="shadow-lg">` |
| `hover:text-purple-400` | Purple text when hovering | `<a class="hover:text-purple-400">` |

### How to Change Colors

**Current**: You want to change the hero section background color from dark gray to darker

**Find the hero section**:
```html
<section id="home" class="relative min-h-screen flex items-center justify-center pt-16 overflow-hidden">
    <div class="absolute inset-0 z-0">
        <!-- Background image -->
    </div>
    <div class="absolute inset-0 bg-gray-900 opacity-75 z-10"></div>
```

**Current overlay color**: `bg-gray-900` with `opacity-75`

**How to change it**:

1. Find `bg-gray-900` in the overlay div
2. Replace with a different color:
   - `bg-gray-950` = even darker gray
   - `bg-black` = pure black
   - `bg-purple-900` = dark purple
3. Example - to make it darker:
```html
<div class="absolute inset-0 bg-gray-950 opacity-75 z-10"></div>
```

### How to Change Button Colors

**Current primary button**:
```html
<a href="https://internetmarketingbrighton.com" target="_blank" rel="noopener noreferrer" class="hover-lift px-8 py-4 bg-gradient-to-r from-purple-600 to-purple-700 text-white font-bold rounded-lg shadow-lg hover:shadow-xl hover:scale-105 transition-all duration-300">
    Get Started Now
</a>
```

**Key color classes**:
- `bg-gradient-to-r from-purple-600 to-purple-700` = gradient background (purple)
- `text-white` = white text
- `hover:shadow-xl` = larger shadow on hover

**How to change button to blue**:

1. Find the button code
2. Replace `from-purple-600 to-purple-700` with `from-blue-600 to-blue-700`
3. Example:
```html
<a href="https://internetmarketingbrighton.com" target="_blank" rel="noopener noreferrer" class="hover-lift px-8 py-4 bg-gradient-to-r from-blue-600 to-blue-700 text-white font-bold rounded-lg shadow-lg hover:shadow-xl hover:scale-105 transition-all duration-300">
    Get Started Now
</a>
```

**Available color options**:
- `blue-600` and `blue-700`
- `green-600` and `green-700`
- `red-600` and `red-700`
- `indigo-600` and `indigo-700`
- `pink-600` and `pink-700`

### How to Change Text Sizes

**Current large heading**:
```html
<h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-bold text-white mb-6 leading-tight tracking-tight">
```

**What these mean**:
- `text-4xl` = size on mobile phones
- `sm:text-5xl` = size on small tablets
- `md:text-6xl` = size on medium screens
- `lg:text-7xl` = size on large screens

**How to make text smaller**:

1. Find the heading you want to change
2. Reduce the numbers by one (e.g., `text-7xl` → `text-6xl`)
3. Example - to make the hero title smaller:
```html
<h1 class="text-3xl sm:text-4xl md:text-5xl lg:text-6xl font-bold text-white mb-6 leading-tight tracking-tight">
```

**Size scale** (from smallest to largest):
- `text-xs`, `text-sm`, `text-base`, `text-lg`, `text-xl`
- `text-2xl`, `text-3xl`, `text-4xl`, `text-5xl`
- `text-6xl`, `text-7xl`, `text-8xl`, `text-9xl`

### How to Change Spacing (Padding & Margins)

**Current button padding**:
```html
<a class="px-8 py-4 ...">
```

**What these mean**:
- `px-8` = horizontal padding (left and right) = 8 units
- `py-4` = vertical padding (top and bottom) = 4 units

**How to make button bigger**:

1. Find `px-8 py-4` in the button
2. Increase the numbers (e.g., `px-8` → `px-12`)
3. Example - to make button larger:
```html
<a class="px-12 py-6 ...">
```

**Spacing scale** (from smallest to largest):
- `0`, `1`, `2`, `3`, `4`, `6`, `8`, `10`, `12`, `16`, `20`, `24`, `28`, `32`

### How to Change Rounded Corners

**Current feature card**:
```html
<div class="... rounded-xl p-8 ...">
```

**What `rounded-xl` means**: Extra large rounded corners

**How to change it**:

1. Find `rounded-xl` in the element
2. Replace with a different value:
   - `rounded-none` = no rounding (square corners)
   - `rounded-sm` = very slightly rounded
   - `rounded-md` = medium rounding
   - `rounded-lg` = large rounding
   - `rounded-full` = completely circular
3. Example - to make corners sharper:
```html
<div class="... rounded-md p-8 ...">
```

### How to Change Shadows

**Current card shadow**:
```html
<div class="... shadow-lg ...">
```

**Shadow options**:
- `shadow-none` = no shadow
- `shadow-sm` = small shadow
- `shadow-md` = medium shadow
- `shadow-lg` = large shadow
- `shadow-xl` = extra large shadow
- `shadow-2xl` = huge shadow

**How to make cards more dramatic**:

1. Find `shadow-lg` in feature cards
2. Change to `shadow-xl` or `shadow-2xl`
3. Example:
```html
<div class="... shadow-2xl ...">
```

### How to Change Opacity (Transparency)

**Current background overlay**:
```html
<div class="absolute inset-0 bg-gray-900 opacity-75 z-10"></div>
```

**What `opacity-75` means**: 75% opaque (25% transparent)

**How to make it more transparent**:

1. Find `opacity-75`
2. Change to a lower number:
   - `opacity-50` = 50% opaque (more see-through)
   - `opacity-25` = 25% opaque (very see-through)
3. Example - to see more of the background image:
```html
<div class="absolute inset-0 bg-gray-900 opacity-50 z-10"></div>
```

**Opacity options**: `opacity-0`, `opacity-5`, `opacity-10`, `opacity-20`, `opacity-25`, `opacity-30`, `opacity-40`, `opacity-50`, `opacity-60`, `opacity-70`, `opacity-75`, `opacity-80`, `opacity-90`, `opacity-95`, `opacity-100`

---

## Fixing and Managing Links

### Understanding Links in Your Page

Links are created using the `<a>` tag. There are three types on your page:

1. **Internal links** (to sections on the same page): `href="#features"`
2. **External links** (to other websites): `href="https://example.com"`
3. **Email links** (to send emails): `href="mailto:email@example.com"`

### Current Links in Your Navigation

**Location**: Search for `<nav>` in the header

**Current navigation links**:
```html
<a href="#home" class="...">Home</a>
<a href="#features" class="...">Features</a>
<a href="#benefits" class="...">Benefits</a>
<a href="#about" class="...">About</a>
<a href="#testimonials" class="...">Testimonials</a>
<a href="#faq" class="...">FAQ</a>
<a href="#contact" class="...">Contact</a>
```

**What's working**: All these links work correctly because they link to section IDs on the same page.

**What might be broken**: If you've deleted or renamed any sections, the links won't work.

### How to Fix a Broken Navigation Link

**Example**: If you deleted the testimonials section

**Find the broken link**:
```html
<a href="#testimonials" class="...">Testimonials</a>
```

**Three options to fix it**:

**Option 1 - Remove the link** (if you don't have that section):
```html
<!-- Delete the entire line -->
```

**Option 2 - Change it to link somewhere else**:
```html
<a href="#benefits" class="...">Testimonials</a>
```

**Option 3 - Recreate the section** with the proper ID:
```html
<section id="testimonials" class="py-24 bg-gray-900">
    <!-- Add your testimonials content here -->
</section>
```

### Current External Links (Links to Other Websites)

**Location**: Search for `https://`

**Current external links**:

1. **"Get Started Now" button in hero section**:
```html
<a href="https://internetmarketingbrighton.com" target="_blank" rel="noopener noreferrer" class="...">
    Get Started Now
</a>
```

2. **"Start Now" button in CTA section**:
```html
<a href="https://internetmarketingbrighton.com" target="_blank" rel="noopener noreferrer" class="...">
    Start Now
</a>
```

3. **"Our Website" link in footer**:
```html
<a href="https://internetmarketingbrighton.com" target="_blank" rel="noopener noreferrer" class="...">
    Our Website
</a>
```

### How to Change External Links

**Current**: You want to change where the "Get Started Now" button links to

**Find the button**:
```html
<a href="https://internetmarketingbrighton.com" target="_blank" rel="noopener noreferrer" class="...">
    Get Started Now
</a>
```

**How to change it**:

1. Find `href="https://internetmarketingbrighton.com"`
2. Replace the URL between the quotes
3. Example - to link to a different website:
```html
<a href="https://yourbrand.com/sleep-guide" target="_blank" rel="noopener noreferrer" class="...">
    Get Started Now
</a>
```

**Keep these attributes the same**:
- `target="_blank"` = opens link in new tab
- `rel="noopener noreferrer"` = security feature for external links

### Current Email Links

**Location**: Search for `mailto:`

**Current email links**:

1. **In CTA section**:
```html
<a href="mailto:internetmarketingbrighton@gmail.com" class="...">
    Contact Us
</a>
```

2. **In footer**:
```html
<a href="mailto:internetmarketingbrighton@gmail.com" class="...">
    internetmarketingbrighton@gmail.com
</a>
```

3. **In footer contact info**:
```html
Email us at <a href="mailto:internetmarketingbrighton@gmail.com" class="...">
    internetmarketingbrighton@gmail.com
</a>
```

### How to Change Email Links

**Current**: You want to change the contact email address

**Find all email links**:

Use `Ctrl+F` (or `Cmd+F`) and search for `mailto:internetmarketingbrighton@gmail.com`

**How to change them**:

1. Replace `internetmarketingbrighton@gmail.com` with your email
2. Example:
```html
<a href="mailto:yourname@yourdomain.com" class="...">
    Contact Us
</a>
```

**Important**: Update the display text too if it shows the email:
```html
<a href="mailto:yourname@yourdomain.com" class="...">
    yourname@yourdomain.com
</a>
```

### Mobile Menu Links

**Location**: Search for `class="mobile-menu"`

**Current mobile menu links**:
```html
<a href="#home" class="block text-gray-300 hover:text-white transition-colors duration-300 py-2 font-medium" onclick="toggleMobileMenu()">Home</a>
<a href="#features" class="block text-gray-300 hover:text-white transition-colors duration-300 py-2 font-medium" onclick="toggleMobileMenu()">Features</a>
<!-- ... more links ... -->
```

**How to update them**:

1. These should match your desktop navigation links
2. Update the `href="#..."` values the same way you would for desktop
3. Keep `onclick="toggleMobileMenu()"` exactly as it is (this closes the menu when clicking)

### Testing Your Links

After updating links, test them:

1. **Save the file** (`Ctrl+S` or `Cmd+S`)
2. **Refresh your browser** (`F5` or `Cmd+R`)
3. **Click each link** to make sure it works:
   - Internal links should scroll to that section
   - External links should open in a new tab
   - Email links should open your email client

---

## Adding Privacy and Terms Pages

### Understanding the Current Link Structure

Your page currently has links to privacy and terms pages that don't exist yet:

**In footer** (search for `privacy.html`):
```html
<a href="privacy.html" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Privacy Policy</a>
<a href="terms.html" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Terms of Service</a>
```

**These links will show a 404 error** because the files don't exist.

### Step 1: Create the Privacy Policy Page

**Create a new file**:

1. Open your text editor
2. Go to **File → New** to create a blank document
3. Save it as `privacy.html` in the same folder as your `index.html`

**Copy this template into privacy.html**:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy for Sleep Guide">
    <title>Privacy Policy - Sleep Guide</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-gray-900 text-gray-100">
    <!-- Header & Navigation -->
    <header class="fixed top-0 w-full bg-gray-900 bg-opacity-95 backdrop-blur-md z-50 border-b border-gray-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <div class="flex items-center space-x-2">
                        <i class="fas fa-moon text-2xl text-purple-500"></i>
                        <span class="text-xl font-bold text-white hidden sm:inline">Sleep Guide</span>
                    </div>
                </div>
                <a href="index.html" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Back to Home</a>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main class="pt-32 pb-20">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl md:text-5xl font-bold text-white mb-8">Privacy Policy</h1>
            
            <div class="prose prose-invert max-w-none text-gray-300 space-y-6">
                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">Introduction</h2>
                    <p>
                        Sleep Guide ("we," "us," "our," or "Company") operates the Sleep Guide website. This page informs you of our policies regarding the collection, use, and disclosure of personal data when you use our Service and the choices you have associated with that data.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">Information Collection and Use</h2>
                    <p>
                        We collect several different types of information for various purposes to provide and improve our Service to you.
                    </p>
                    <h3 class="text-xl font-semibold text-white mt-6 mb-3">Types of Data Collected:</h3>
                    <ul class="list-disc list-inside space-y-2 ml-4">
                        <li>Personal Data: Email address, name, phone number (if you contact us)</li>
                        <li>Usage Data: Browser type, IP address, pages visited, time spent on pages</li>
                        <li>Cookies: Small files stored on your device to remember your preferences</li>
                    </ul>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">Use of Data</h2>
                    <p>Sleep Guide uses the collected data for various purposes:</p>
                    <ul class="list-disc list-inside space-y-2 ml-4">
                        <li>To provide and maintain our Service</li>
                        <li>To notify you about changes to our Service</li>
                        <li>To allow you to participate in interactive features</li>
                        <li>To provide customer support</li>
                        <li>To gather analysis or valuable information so that we can improve our Service</li>
                        <li>To monitor the usage of our Service</li>
                        <li>To detect, prevent and address technical issues</li>
                    </ul>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">Security of Data</h2>
                    <p>
                        The security of your data is important to us but remember that no method of transmission over the Internet or method of electronic storage is 100% secure. While we strive to use commercially acceptable means to protect your Personal Data, we cannot guarantee its absolute security.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">Contact Us</h2>
                    <p>
                        If you have any questions about this Privacy Policy, please contact us at:
                    </p>
                    <p class="mt-4">
                        Email: <a href="mailto:internetmarketingbrighton@gmail.com" class="text-purple-400 hover:text-purple-300">internetmarketingbrighton@gmail.com</a>
                    </p>
                </section>
            </div>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 border-t border-gray-800 py-8">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-gray-400 text-sm">
                &copy; 2024 Sleep Guide. All rights reserved.
            </p>
        </div>
    </footer>
</body>
</html>
```

### Step 2: Create the Terms of Service Page

**Create a new file**:

1. Open your text editor
2. Go to **File → New**
3. Save it as `terms.html` in the same folder as your `index.html`

**Copy this template into terms.html**:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service for Sleep Guide">
    <title>Terms of Service - Sleep Guide</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-gray-900 text-gray-100">
    <!-- Header & Navigation -->
    <header class="fixed top-0 w-full bg-gray-900 bg-opacity-95 backdrop-blur-md z-50 border-b border-gray-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <div class="flex items-center space-x-2">
                        <i class="fas fa-moon text-2xl text-purple-500"></i>
                        <span class="text-xl font-bold text-white hidden sm:inline">Sleep Guide</span>
                    </div>
                </div>
                <a href="index.html" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Back to Home</a>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main class="pt-32 pb-20">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl md:text-5xl font-bold text-white mb-8">Terms of Service</h1>
            
            <div class="prose prose-invert max-w-none text-gray-300 space-y-6">
                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">1. Terms</h2>
                    <p>
                        By accessing and using this website, you accept and agree to be bound by the terms and provision of this agreement. If you do not agree to abide by the above, please do not use this service.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">2. Use License</h2>
                    <p>
                        Permission is granted to temporarily download one copy of the materials (information or software) on Sleep Guide's website for personal, non-commercial transitory viewing only. This is the grant of a license, not a transfer of title, and under this license you may not:
                    </p>
                    <ul class="list-disc list-inside space-y-2 ml-4">
                        <li>Modifying or copying the materials</li>
                        <li>Using the materials for any commercial purpose or for any public display</li>
                        <li>Attempting to decompile or reverse engineer any software contained on the website</li>
                        <li>Removing any copyright or other proprietary notations from the materials</li>
                        <li>Transferring the materials to another person or "mirroring" the materials on any other server</li>
                    </ul>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">3. Disclaimer</h2>
                    <p>
                        The materials on Sleep Guide's website are provided on an 'as is' basis. Sleep Guide makes no warranties, expressed or implied, and hereby disclaims and negates all other warranties including, without limitation, implied warranties or conditions of merchantability, fitness for a particular purpose, or non-infringement of intellectual property or other violation of rights.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">4. Limitations</h2>
                    <p>
                        In no event shall Sleep Guide or its suppliers be liable for any damages (including, without limitation, damages for loss of data or profit, or due to business interruption) arising out of the use or inability to use the materials on Sleep Guide's website.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">5. Accuracy of Materials</h2>
                    <p>
                        The materials appearing on Sleep Guide's website could include technical, typographical, or photographic errors. Sleep Guide does not warrant that any of the materials on its website are accurate, complete, or current. Sleep Guide may make changes to the materials contained on its website at any time without notice.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">6. Links</h2>
                    <p>
                        Sleep Guide has not reviewed all of the sites linked to its website and is not responsible for the contents of any such linked site. The inclusion of any link does not imply endorsement by Sleep Guide of the site. Use of any such linked website is at the user's own risk.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">7. Modifications</h2>
                    <p>
                        Sleep Guide may revise these terms of service for its website at any time without notice. By using this website, you are agreeing to be bound by the then current version of these terms of service.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">8. Governing Law</h2>
                    <p>
                        These terms and conditions are governed by and construed in accordance with the laws of the jurisdiction in which Sleep Guide operates, and you irrevocably submit to the exclusive jurisdiction of the courts in that location.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mt-8 mb-4">9. Contact Information</h2>
                    <p>
                        If you have any questions about these Terms of Service, please contact us at:
                    </p>
                    <p class="mt-4">
                        Email: <a href="mailto:internetmarketingbrighton@gmail.com" class="text-purple-400 hover:text-purple-300">internetmarketingbrighton@gmail.com</a>
                    </p>
                </section>
            </div>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 border-t border-gray-800 py-8">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-gray-400 text-sm">
                &copy; 2024 Sleep Guide. All rights reserved.
            </p>
        </div>
    </footer>
</body>
</html>
```

### Step 3: Verify the Links Work

**Test your setup**:

1. **Save all files** in the same folder:
   - `index.html`
   - `privacy.html`
   - `terms.html`

2. **Open index.html** in your browser

3. **Scroll to the footer** and click "Privacy Policy"
   - Should open the privacy page

4. **Click "Back to Home"** at the top of the privacy page
   - Should return to index.html

5. **Repeat for Terms of Service**

### Step 4: Customize the Privacy and Terms Pages

**Update company name and email**:

In both `privacy.html` and `terms.html`, find and replace:
- `internetmarketingbrighton@gmail.com` → your email
- `Sleep Guide` → your company name (if different)

**Add your specific policies**:

1. Open `privacy.html`
2. Find the section that says "Types of Data Collected:"
3. Update the bullet points to match what data you actually collect
4. Add any additional privacy information specific to your business

**Example - updating privacy policy**:

Current:
```html
<li>Personal Data: Email address, name, phone number (if you contact us)</li>
```

Updated:
```html
<li>Personal Data: Email address, name, phone number, sleep tracking data (if you contact us)</li>
```

### Step 5: Update Footer Links (Optional But Recommended)

**Current footer links**:
```html
<a href="privacy.html" class="...">Privacy Policy</a>
<a href="terms.html" class="...">Terms of Service</a>
```

These already work! But if you want to make them more prominent or add them to navigation, you can add similar links in the desktop or mobile navigation menus.

### Alternative: Using Existing Pages

If you already have privacy and terms pages hosted elsewhere (like a blog or separate domain), you can update the links:

**Change**:
```html
<a href="privacy.html" class="...">Privacy Policy</a>
```

**To**:
```html
<a href="https://yourdomain.com/privacy" target="_blank" rel="noopener noreferrer" class="...">Privacy Policy</a>
```

**Important**: Add `target="_blank" rel="noopener noreferrer"` if linking to external websites so the link opens in a new tab.

---

## Common Customizations

### Adding a New Section

**Example**: You want to add a "Pricing" section between Features and Benefits

**Step 1 - Find where to add it**:

Search for `id="benefits"` to find the benefits section. You'll add your new section before it.

**Step 2 - Create the section HTML**:

```html
<!-- Pricing Section -->
<section id="pricing" class="py-24 bg-gray-800 relative">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center mb-16">
            <h2 class="text-3xl sm:text-4xl md:text-5xl font-bold text-white mb-4 leading-tight">
                Simple, Transparent Pricing
            </h2>
            <p class="text-xl text-gray-400 max-w-2xl mx-auto">
                Choose the plan that works best for you
            </p>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <!-- Pricing Card 1 -->
            <div class="bg-gray-900 border border-gray-700 rounded-xl p-8">
                <h3 class="text-2xl font-bold text-white mb-4">Basic</h3>
                <div class="text-4xl font-bold text-purple-400 mb-4">$9<span class="text-lg text-gray-400">/month</span></div>
                <ul class="space-y-3 mb-8 text-gray-300">
                    <li class="flex items-center">
                        <i class="fas fa-check text-purple-400 mr-3"></i>
                        <span>Sleep guide access</span>
                    </li>
                    <li class="flex items-center">
                        <i class="fas fa-check text-purple-400 mr-3"></i>
                        <span>Email support</span>
                    </li>
                </ul>
                <button class="w-full px-6 py-3 bg-purple-600 text-white font-bold rounded-lg hover:bg-purple-700 transition-colors duration-300">
                    Get Started
                </button>
            </div>
        </div>
    </div>
</section>
```

**Step 3 - Add to navigation**:

Find the desktop navigation and add:
```html
<a href="#pricing" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Pricing</a>
```

Find the mobile menu and add:
```html
<a href="#pricing" class="block text-gray-300 hover:text-white transition-colors duration-300 py-2 font-medium" onclick="toggleMobileMenu()">Pricing</a>
```

### Changing the Hero Background Image

**Current image**:
```html
<img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=1200&h=800&fit=crop" alt="Sleep background" class="w-full h-full object-cover opacity-25">
```

**How to change it**:

1. Find a new image on Unsplash (unsplash.com) or Pexels (pexels.com)
2. Copy the image URL
3. Replace the URL in `src="..."`
4. Update the `alt` text to describe the new image

**Example**:
```html
<img src="https://images.unsplash.com/photo-1541746972996-4e0b6dfe56cb?w=1200&h=800&fit=crop" alt="Person sleeping peacefully" class="w-full h-full object-cover opacity-25">
```

### Changing Feature Icons

**Current Feature 1 icon**:
```html
<i class="fas fa-dumbbell text-white text-2xl"></i>
```

**How to change it**:

1. Go to Font Awesome website (fontawesome.com)
2. Search for an icon you want
3. Copy the icon class name (e.g., `fa-heart`)
4. Replace `fa-dumbbell` with your new icon

**Example - to use a heart icon**:
```html
<i class="fas fa-heart text-white text-2xl"></i>
```

**Available icons** used in this page:
- `fa-moon` = moon
- `fa-dumbbell` = weights
- `fa-capsules` = pills/supplements
- `fa-bed` = bed
- `fa-star` = star
- `fa-check` = checkmark
- `fa-heart` = heart
- `fa-lightning-bolt` = lightning bolt

### Adding a New Feature Card

**Current feature cards** are in the Features section (search for `id="features"`)

**How to add a new card**:

1. Find the last `</div>` that closes a feature card
2. Copy an entire feature card block
3. Paste it right after the last card
4. Update the text and icon

**Example**:
```html
<!-- Feature 4: Meditation -->
<div class="hover-lift group bg-gray-800 border border-gray-700 rounded-xl p-8 transition-all duration-300 hover:border-purple-500 hover:bg-gray-750">
    <div class="w-16 h-16 bg-gradient-to-br from-purple-500 to-purple-600 rounded-lg flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
        <i class="fas fa-om text-white text-2xl"></i>
    </div>
    <h3 class="text-2xl font-bold text-white mb-4">Meditation Practice</h3>
    <p class="text-gray-400 leading-relaxed mb-4">
        Daily meditation reduces stress and anxiety, making it easier to fall asleep naturally.
    </p>
    <ul class="space-y-2 text-gray-300">
        <li class="flex items-center">
            <i class="fas fa-check text-purple-400 mr-3"></i>
            <span>10 minutes daily</span>
        </li>
        <li class="flex items-center">
            <i class="fas fa-check text-purple-400 mr-3"></i>
            <span>Guided meditation apps</span>
        </li>
        <li class="flex items-center">
            <i class="fas fa-check text-purple-400 mr-3"></i>
            <span>Breathing techniques</span>
        </li>
    </ul>
</div>
```

**Important**: If you add a 4th feature, the grid layout might need adjustment:
- Current: `grid-cols-1 md:grid-cols-2 lg:grid-cols-3` (3 columns on large screens)
- For 4 features, you might want to change to `lg:grid-cols-2` (2 columns) or keep 3 and have one wrap

### Adding a New Testimonial

**Current testimonials** are in the Testimonials section (search for `id="testimonials"`)

**How to add one**:

1. Find the last testimonial card
2. Copy the entire `<div>` block
3. Paste it after the last testimonial
4. Update the review text, name, and title

**Example**:
```html
<div class="hover-lift bg-gray-800 border border-gray-700 rounded-xl p-8 transition-all duration-300 hover:border-purple-500">
    <div class="flex items-center mb-4">
        <div class="flex text-yellow-400">
            <i class="fas fa-star"></i>
            <i class="fas fa-star"></i>
            <i class="fas fa-star"></i>
            <i class="fas fa-star"></i>
            <i class="fas fa-star"></i>
        </div>
        <span class="ml-2 text-gray-400 font-semibold">5.0</span>
    </div>
    <p class="text-gray-300 leading-relaxed mb-6 text-lg">
        "This guide completely changed my approach to sleep. I'm now getting 8 hours every night!"
    </p>
    <div class="border-t border-gray-700 pt-4">
        <p class="text-white font-bold">Alex Johnson</p>
        <p class="text-purple-400 text-sm">Freelance Writer, Seattle</p>
    </div>
</div>
```

### Adding a New FAQ Question

**Current FAQs** are in the FAQ section (search for `id="faq"`)

**How to add one**:

1. Find the last FAQ accordion item
2. Copy the entire accordion `<div>` block
3. Paste it after the last FAQ
4. Update the question and answer

**Example**:
```html
<div class="bg-gray-900 border border-gray-700 rounded-lg overflow-hidden hover:border-purple-500 transition-colors duration-300">
    <button class="accordion-btn w-full px-6 py-4 flex justify-between items-center hover:bg-gray-850 transition-colors duration-300" onclick="toggleAccordion(this)">
        <h3 class="text-lg font-bold text-white text-left">What if I travel across time zones?</h3>
        <i class="fas fa-chevron-down text-purple-400"></i>
    </button>
    <div class="accordion-content px-6 pb-4 text-gray-400">
        <p class="leading-relaxed">
            When traveling, try to gradually adjust your sleep schedule 2-3 days before departure. Use light exposure to help reset your circadian rhythm in the new time zone.
        </p>
    </div>
</div>
```

### Changing Social Media Links

**Current social links** are in the footer (search for `fab fa-facebook`)

**Current links**:
```html
<a href="#" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">
    <i class="fab fa-facebook text-xl"></i>
</a>
```

**How to update them**:

1. Replace `href="#"` with your social media URL
2. Example - Facebook:
```html
<a href="https://facebook.com/yourpage" target="_blank" rel="noopener noreferrer" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">
    <i class="fab fa-facebook text-xl"></i>
</a>
```

**Available social icons**:
- `fab fa-facebook` = Facebook
- `fab fa-twitter` = Twitter/X
- `fab fa-instagram` = Instagram
- `fab fa-youtube` = YouTube
- `fab fa-linkedin` = LinkedIn
- `fab fa-tiktok` = TikTok

---

## Troubleshooting

### Issue: Changes Don't Appear When I Refresh

**Cause**: Browser cache (the browser is showing old version)

**Solution**:
1. **Hard refresh** your browser:
   - Windows: Press `Ctrl+Shift+R`
   - Mac: Press `Cmd+Shift+R`
2. **Clear browser cache**:
   - Open browser settings
   - Find "Clear browsing data"
   - Select "Cached images and files"
   - Click "Clear data"
3. **Try a different browser** to test

### Issue: Links Are Broken (404 Error)

**Cause**: The link points to a file that doesn't exist

**Solution**:
1. **Check file names**:
   - Make sure `privacy.html` and `terms.html` exist in the same folder as `index.html`
   - File names are case-sensitive on some systems
2. **Verify href values**:
   - Make sure `href="privacy.html"` matches the actual filename
3. **Use absolute paths**:
   - Instead of `href="privacy.html"`, try `href="./privacy.html"`

### Issue: Text Is Cut Off or Overlapping

**Cause**: Text is too long for the container

**Solution**:
1. **Reduce text length**: Make paragraphs shorter
2. **Increase container width**: Change `max-w-2xl` to `max-w-3xl` or `max-w-4xl`
3. **Reduce font size**: Change `text-lg` to `text-base` or `text-sm`

**Example**:
```html
<!-- Before -->
<p class="text-lg text-gray-400 max-w-2xl mx-auto">Your very long text here...</p>

<!-- After -->
<p class="text-base text-gray-400 max-w-3xl mx-auto">Your very long text here...</p>
```

### Issue: Images Not Loading

**Cause**: Image URL is broken or incorrect

**Solution**:
1. **Test the image URL**:
   - Copy the URL from `src="..."`
   - Paste it into your browser address bar
   - If the image doesn't load, the URL is broken
2. **Find a new image**:
   - Go to Unsplash.com or Pexels.com
   - Search for your topic
   - Right-click the image and copy the URL
3. **Update the src**:
```html
<img src="https://new-image-url-here.jpg" alt="Description">
```

### Issue: Mobile Menu Doesn't Close

**Cause**: JavaScript issue

**Solution**:
1. **Make sure you didn't delete the JavaScript** at the bottom of the page
2. **Check that all closing tags are intact**:
   - Each `<button>` should have a `</button>`
   - Each `<div>` should have a `</div>`
3. **Verify the onclick attribute**:
```html
<button class="mobile-menu-button md:hidden text-white focus:outline-none" onclick="toggleMobileMenu()">
```

### Issue: Colors Look Wrong

**Cause**: You changed the wrong color class

**Solution**:
1. **Identify the element**:
   - Right-click on the element in your browser
   - Select "Inspect" or "Inspect Element"
   - Look at the HTML to find the class names
2. **Find the class in your code**:
   - Search for that class name in your HTML
   - Make sure you're changing the right element
3. **Use the correct color format**:
   - `bg-purple-600` = background color
   - `text-purple-600` = text color
   - `border-purple-600` = border color

### Issue: Accordion Buttons Don't Work

**Cause**: JavaScript is missing or broken

**Solution**:
1. **Check the JavaScript** at the bottom of the page:
```html
<script>
    function toggleAccordion(button) {
        // This code should be present
    }
</script>
```

2. **Make sure the button has the correct onclick**:
```html
<button class="accordion-btn ..." onclick="toggleAccordion(this)">
```

3. **Verify the accordion content div exists**:
```html
<div class="accordion-content ...">
    <!-- Content here -->
</div>
```

### Issue: Page Looks Different on Mobile

**Cause**: Responsive design is working correctly, but you want to adjust it

**Solution**:

Tailwind CSS uses breakpoints for responsive design:
- `sm:` = small screens (640px+)
- `md:` = medium screens (768px+)
- `lg:` = large screens (1024px+)
- `xl:` = extra large (1280px+)

Example - to change how text sizes on mobile:

```html
<!-- Current -->
<h1 class="text-4xl sm:text-5xl md:text-6xl">

<!-- Smaller on mobile -->
<h1 class="text-2xl sm:text-4xl md:text-5xl">
```

### Issue: Footer Links Go to Wrong Pages

**Cause**: Wrong href values

**Solution**:
1. **Check the href value**:
```html
<a href="privacy.html">Privacy</a>
```

2. **Make sure the file exists**:
   - Open your file explorer
   - Check that `privacy.html` is in the same folder as `index.html`

3. **Test each link**:
   - Click the link
   - See where it takes you
   - Verify it's the correct page

### Issue: Styling Looks Broken After Changes

**Cause**: You accidentally deleted or modified a Tailwind class

**Solution**:
1. **Compare with original**:
   - Open the original HTML file
   - Find the section you changed
   - Compare the class names
2. **Restore missing classes**:
   - If a class is missing, add it back
   - Make sure all classes are separated by spaces
3. **Example of correct format**:
```html
<!-- Correct -->
<div class="bg-gray-900 border border-gray-700 rounded-xl p-8">

<!-- Incorrect - missing space -->
<div class="bg-gray-900border border-gray-700 rounded-xl p-8">
```

### Issue: Form or Contact Button Doesn't Work

**Cause**: Email link or form action is not set up

**Current setup**: The page uses email links (`mailto:`) which open your default email client

**If this isn't working**:
1. **Make sure you have an email client installed** (Outlook, Gmail, etc.)
2. **Or, set up a contact form** instead:
   - Use a service like Formspree, Basin, or Netlify Forms
   - Replace the email link with a form

**Example - using Formspree**:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" class="space-y-4">
    <input type="email" name="email" placeholder="Your email" required class="w-full px-4 py-2 bg-gray-800 border border-gray-700 rounded-lg text-white">
    <textarea name="message" placeholder="Your message" required class="w-full px-4 py-2 bg-gray-800 border border-gray-700 rounded-lg text-white"></textarea>
    <button type="submit" class="px-8 py-3 bg-purple-600 text-white font-bold rounded-lg">Send Message</button>
</form>
```

---

## Quick Reference: File Structure

Your project should look like this:

```
project-folder/
├── index.html          (main landing page)
├── privacy.html        (privacy policy page)
├── terms.html          (terms of service page)
└── blog.html           (optional - for blog link in footer)
```

**All files should be in the same folder** so links work correctly.

---

## Final Checklist Before Deployment

Before publishing your site, verify:

- [ ] All text has been customized
- [ ] All links have been tested and work correctly
- [ ] Email address has been updated
- [ ] Social media links are correct
- [ ] Images are loading properly
- [ ] Mobile menu works on phone/tablet
- [ ] All sections scroll smoothly
- [ ] Privacy policy page exists and links work
- [ ] Terms of service page exists and links work
- [ ] No broken links (test every link)
- [ ] Page looks good on mobile, tablet, and desktop
- [ ] All buttons and forms work

---

## Additional Resources

### Learning HTML & CSS

- **MDN Web Docs**: https://developer.mozilla.org/en-US/docs/Web/HTML
- **W3Schools**: https://www.w3schools.com/html/
- **Tailwind CSS Docs**: https://tailwindcss.com/docs

### Finding Images

- **Unsplash**: https://unsplash.com
- **Pexels**: https://www.pexels.com
- **Pixabay**: https://pixabay.com

### Icons

- **Font Awesome**: https://fontawesome.com/icons

### Tools

- **VS Code**: https://code.visualstudio.com
- **Color Picker**: https://htmlcolorcodes.com
- **Responsive Tester**: https://responsivedesignchecker.com

---

## Support

If you encounter issues not covered in this guide:

1. **Check the code carefully** for typos
2. **Use browser developer tools** (F12) to see error messages
3. **Compare with the original** HTML to spot differences
4. **Test one change at a time** to isolate problems
5. **Make backups** before making major changes

Remember: Take your time, make one change at a time, and test frequently. Happy customizing!