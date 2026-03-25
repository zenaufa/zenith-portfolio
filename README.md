<p align="center">
  <img src=https://github.com/zenaufa/zenith-portfolio/blob/main/Preview.gif>
</p>

# Zenith Portfolio

A sleek, single-page, highly interactive personal portfolio template designed to showcase your work experience, certifications, and professional activities. It features smooth scrolling, dynamic color adaptations, and engaging background effects to make your profile stand out.

## ✨ Features

* **Responsive Design**: Looks great on desktops, tablets, and mobile devices.
* **SEO Optimized**: Includes Open Graph tags, Twitter Cards, and Schema.org JSON-LD structured data to help your portfolio rank well in search engines.
* **Interactive Hero Section**: 
    * Animated "typing" effect for your job roles.
    * Interactive `particles.js` background.
    * Floating, glowing orbs.
* **Dynamic Color Adaptation**: The accent colors of the glowing orbs dynamically change based on the dominant colors of the images you hover over or view in the carousels.
* **Smooth Scrolling**: Powered by Lenis.js for a premium, buttery-smooth scrolling experience.
* **Custom Carousels**: 
    * **Testimonials**: Auto-sliding and interactive carousel in the hero section.
    * **Project Imagery**: Swipeable/clickable image carousels for your experience and activity items.
* **Scroll Progress Indicator**: A fixed progress bar at the top of the screen tracks the user's reading progress.

## 🚀 How to Use & Customize

This template is designed to be easily updated without needing to dig deep into complex HTML structures. Most of your content is managed via simple JavaScript arrays.

### 1. Basic Setup (HTML & SEO)
Open `index.html` and update the head section to reflect your information:
* **Page Title & Meta Tags**: Update `<title>`, `<meta name="description">`, and `<meta name="author">`.
* **Social Tags (Open Graph/Twitter)**: Update the `og:title`, `og:description`, `og:image`, and `og:url` tags so your link looks good when shared on LinkedIn or Twitter.
* **Schema.org JSON**: Update your name, job titles, and location in the `<script type="application/ld+json">` blocks.

### 2. Update the Hero Section
Scroll down to the `<section class="hero">` block in the HTML:
* Replace the `src` of the profile picture inside `<div class="hero-image">`.
* Update the `<h1>` tag with your name.
* Update the `href` attribute in the `<a class="connect-btn">` to point to your LinkedIn, email, or contact page.

### 3. Customize Your Content (The Data)
Scroll down to the `<script>` tag titled `CONTENT DATA` (around line 430). Here, you can easily edit the data arrays to populate the site:

* **`CONFIG.roles`**: Update this array with the different job titles or skills you want to animate under your name in the hero section.
* **`experienceData`**: Add your past and current jobs here. Include your title, company, dates, a brief description, and relevant images.
* **`trainingData`**: List your certifications, degrees, or courses.
* **`activitiesData`**: Add your speaking gigs, hackathons, open-source contributions, or community involvement.
* **`testimonialData`**: Add quotes and author details for the hero section's review carousel.

### 4. Adjust the Colors (Optional)
If you want to change the default color scheme, scroll to the `<style>` block at the top of the file and locate the `:root` variables:
```css
:root {
    --orb1-color: #a855f7;
    --orb2-color: #ec4899;
    --orb3-color: #06b6d4;
    --bg-primary: #0a0a0a;
    --accent-purple: #4c2295;
    /* Change these hex codes to match your personal brand! */
}
