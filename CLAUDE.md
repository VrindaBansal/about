# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal portfolio website for Vrinda Bansal built as a single-page application using vanilla HTML, CSS, and JavaScript. The site features a GitHub-inspired design with interactive elements and is deployed via GitHub Pages.

## Architecture

The entire application is contained within a single `index.html` file that includes:

- **Embedded CSS**: All styling is contained within `<style>` tags in the document head
- **Inline JavaScript**: All interactive functionality is in a `<script>` tag at the end of the body
- **Static Assets**: Profile images (DSC_0010.JPG, 1592599892797.jpeg) and favicon.png are referenced locally

### Key Components

- **Header/Navigation**: Fixed navigation with smooth scrolling to sections
- **Sidebar Profile**: Personal information, bio with typing effect, socials (including GitHub), and contact links
- **Experience Section**: Interactive cards with modal popups showing detailed experience information
- **Projects Section**: Featured projects with external links
- **Education Section**: Educational background display

### Interactive Features

- **Experience Modals**: Clicking experience cards opens detailed modal popups with achievements and tech stacks
- **Smooth Scrolling**: Navigation links scroll smoothly to corresponding sections
- **Animations**: Intersection Observer for card animations, typing effect for bio text, floating particles background
- **Responsive Design**: Mobile-friendly layout using CSS Grid and media queries

## Deployment

The site is deployed via GitHub Pages and accessible at `https://vrindabansal.github.io/about/`

## Development Notes

- No build process or package manager - pure static HTML/CSS/JS
- Profile image path references `/about/DSC_0010.JPG` for GitHub Pages deployment
- All external dependencies loaded via CDN (Font Awesome icons)
- Experience data is stored in JavaScript object `experienceData` for modal content

## Development Workflow

Since this is a static site with no build process:
- All changes are made directly to `index.html`
- CSS is embedded in `<style>` tags within the document head
- JavaScript is embedded in `<script>` tags at the end of the body
- Static assets (images, favicon) are referenced with `/about/` prefix for GitHub Pages compatibility
- Test changes locally by opening `index.html` in a browser
- Deploy by pushing to the `main` branch (automatic via GitHub Pages)

## Code Architecture

### Single-File Structure
- **HTML Structure**: Semantic layout with header, sidebar, and main content areas
- **CSS Styling**: GitHub-inspired dark theme with responsive grid layout and animations
- **JavaScript Functionality**: Interactive modal system, smooth scrolling, typing effects, and particle animations

### Key JavaScript Components
- `experienceData` object: Contains detailed information for modal popups
- Modal system: Handles experience card interactions and detailed views
- Animation system: Intersection Observer for scroll-triggered animations, typing effects, and floating particles
- Navigation: Smooth scrolling between sections

### Data Management
- Experience details stored in JavaScript object for modal content
- Skills organized by categories with proficiency levels (expert, advanced, intermediate, beginner)
- No external data sources or APIs

## Asset Requirements

- Profile images must be sized appropriately (260px x 260px for main profile)
- All image paths use `/about/` prefix for GitHub Pages deployment
- Font Awesome icons loaded via CDN for UI elements

## Recent Updates

- Fixed Roadmap project URL to point to correct Vercel deployment
- Changed "Achievements" section to "Socials" with GitHub profile link added
- Cleaned up duplicate code that was previously at the end of index.html