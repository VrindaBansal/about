# Assets Directory

This directory contains all optimized images used across the portfolio website.

## Structure

```
assets/
├── images/
│   ├── favicons/          # Small navigation icons (28x28px, optimized)
│   │   ├── github.png     # GitHub version favicon (8.4KB)
│   │   ├── notion.png     # Notion version favicon (4.6KB)
│   │   └── figma.png      # Figma version favicon (2.7KB)
│   ├── profile/           # Profile photos and related images
│   │   ├── DSC_0010_optimized.jpg  # Main profile image (68KB, 800px max)
│   │   └── 1592599892797.jpeg      # Secondary profile image (69KB)
│   ├── banners/           # Page banner images
│   │   └── notion.jpg     # Notion page banner (174KB, 1200px max)
│   └── posters/           # 1200px poster previews rendered from the PDFs in posters/
├── papers/                # Paper PDFs linked from research/
│   └── carecart-paper.pdf
├── posters/               # Original research poster PDFs linked from research/
```

## Optimization Details

All images have been optimized for web performance:

- **Profile images**: Resized to appropriate dimensions (≤800px) while maintaining quality
- **Favicons**: Standardized to 28x28px for consistent UI
- **Banners**: Optimized for display while keeping file sizes minimal
- **Total size reduction**: ~15MB → ~340KB (97.7% reduction)

## Usage

Images are referenced with paths like:
- `/about/assets/images/profile/DSC_0010_optimized.jpg`
- `../assets/images/favicons/github.png`
- `assets/images/banners/notion.jpg`