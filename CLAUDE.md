# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-page web application that generates Final Fantasy XIV-style trial title screens. The application is built using vanilla HTML, CSS, and JavaScript with no build system or external dependencies beyond Google Fonts.

## Development Setup

No build process or package manager required. Simply open `index.html` in a modern web browser.

## Architecture

- **Single File Application**: Everything is contained in `index.html` - HTML structure, CSS styles, and JavaScript functionality
- **SVG-based Rendering**: Uses SVG for title screen generation, allowing for crisp vector graphics and easy serialization
- **Client-side Image Processing**: Handles background image uploads and converts SVG to PNG for download using Canvas API
- **Static Asset Dependencies**: Requires `back-image.jpg` for default background and `ogp-image.jpg` for social media previews

## Core Components

### Text Input System
- Three text inputs: subtitle (top), English main title, and Japanese title
- Real-time preview updates as users type
- Default values: "FFXIV", "Trial Title Generator", "FF14討滅戦タイトル風画面ジェネレーター"

### Background System
- Default background: `back-image.jpg` (must be present in project root)
- Custom background image upload with File API
- Images embedded as data URLs with 40% dark overlay for text readability

### SVG Generation Engine
- Dynamic SVG creation with complex gradients, filters, and effects
- FF14-style typography using Cinzel (English) and Noto Serif JP (Japanese) fonts
- Advanced text effects including bevel, glow, and shadow filters
- Fixed output resolution of 1920x1080 pixels

### Export Functionality
- SVG to PNG conversion using Canvas API
- Automatic download trigger with filename `ff14-title.png`

## Static Assets

### Required Files
- `back-image.jpg`: Default background image (1920x1080 recommended)
- `ogp-image.jpg`: Social media preview image (1200x630px)

### Social Media Integration
- Comprehensive Open Graph Protocol (OGP) meta tags
- Twitter Card support with large image format
- Static preview image configured for consistent social sharing

## Font Dependencies

- **Cinzel**: Used for English titles and decorative text
- **Noto Serif JP**: Used for Japanese text to ensure proper character rendering
- Both loaded from Google Fonts CDN

## Browser Compatibility

Requires modern browser features:
- SVG support with advanced filters
- Canvas API for image export
- File API for image uploads
- Blob and URL APIs for downloads