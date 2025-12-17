# Image Privacy Guard

Image Privacy Guard is a lightweight, privacy-focused web tool that analyzes image metadata entirely in the browser. It helps users identify and remove privacy-sensitive information before sharing images online without uploading files to any server.

## Features

### Client-Side Metadata Risk Analyzer

- **🔍 Scans uploaded images for privacy-sensitive metadata**
  - GPS coordinates (latitude, longitude, location data)
  - Device information (make, model, serial numbers)
  - Personal information (artist, author, copyright, creator)
  - Timestamps (DateTime, DateTimeOriginal, DateTimeDigitized)
  - Software and host computer information

- **⚠️ Flags sensitive metadata with risk indicators**
  - Visual warnings for privacy-sensitive fields
  - Automatic detection of potentially identifying information
  - Clear categorization of metadata types

- **📊 Provides comprehensive risk scoring**
  - **High Risk**: Images with GPS coordinates or 5+ sensitive fields
  - **Medium Risk**: Images with 2-4 sensitive fields
  - **Low Risk**: Images with 0-1 sensitive fields

- **🗑️ One-click removal of selected metadata fields**
  - Select individual fields to remove
  - "Select All Sensitive" button for quick removal of all risky data
  - Client-side processing ensures privacy
  - Download cleaned images with metadata stripped

- **🔐 100% Privacy-Focused**
  - All processing happens in your browser
  - No server uploads
  - No data collection
  - No external API calls

## Usage

1. Open `index.html` in your web browser
2. Click or drag an image onto the upload area
3. Review the metadata analysis and risk score
4. Select which metadata fields to remove (sensitive fields are pre-selected)
5. Click "Remove Selected Metadata" to clean the image
6. Download your privacy-protected image

## Supported Image Formats

- JPEG/JPG (with EXIF metadata support)
- PNG
- Other image formats supported by browsers

## Technical Details

- Pure HTML, CSS, and JavaScript
- No external dependencies or libraries required
- Custom EXIF parser for metadata extraction
- Canvas API for metadata removal
- Responsive design for mobile and desktop

## Security & Privacy

This tool prioritizes your privacy:
- ✅ All operations are performed locally in your browser
- ✅ Images never leave your device
- ✅ No server-side processing
- ✅ No tracking or analytics
- ✅ Open source and auditable

## Demo

Simply open the `index.html` file in any modern web browser. No build process or installation required.

## License

See LICENSE file for details.
