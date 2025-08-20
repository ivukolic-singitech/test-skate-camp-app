# Camp Rollerblade LOZ 2025 - PWA Deployment Guide

## Files Required for GitHub Pages Deployment

To deploy this PWA to `https://ivukolic-singitech.github.io/skate-camp-loz/`, you need to upload the following files to your GitHub repository:

### Required Files:
1. **index.html** - Main application file (from the first artifact)
2. **manifest.json** - PWA manifest file (from the second artifact)
3. **sw.js** - Service worker for offline functionality (from the third artifact)
4. **Icons** - App icons in various sizes (you'll need to create these)

## Step-by-Step Deployment Process

### 1. Create App Icons
You'll need to create app icons from the Camp Rollerblade logo in the following sizes:
- icon-72.png (72x72px)
- icon-96.png (96x96px)
- icon-128.png (128x128px)
- icon-144.png (144x144px)
- icon-152.png (152x152px)
- icon-192.png (192x192px)
- icon-384.png (384x384px)
- icon-512.png (512x512px)

**How to create icons:**
1. Download the logo from: `https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/file-uploads/themes/2156834118/settings_images/0f3b800-37e2-38c1-2856-18f411532cda_Camp_Rollerblade.png`
2. Use an online tool like [PWA Icon Generator](https://www.pwabuilder.com/imageGenerator) or image editing software
3. Create square icons with rounded corners and proper padding
4. Save as PNG files with the names listed above

### 2. Upload to GitHub Repository
1. Navigate to your GitHub repository: `ivukolic-singitech/skate-camp-loz`
2. Upload the following files to the root directory:
   ```
   /
   ├── index.html
   ├── manifest.json
   ├── sw.js
   ├── icon-72.png
   ├── icon-96.png
   ├── icon-128.png
   ├── icon-144.png
   ├── icon-152.png
   ├── icon-192.png
   ├── icon-384.png
   └── icon-512.png
   ```

### 3. Enable GitHub Pages
1. Go to repository Settings
2. Scroll to "Pages" section
3. Select "Deploy from a branch"
4. Choose "main" branch and "/ (root)" folder
5. Click "Save"

### 4. Verify Deployment
1. Wait a few minutes for deployment
2. Visit: `https://ivukolic-singitech.github.io/skate-camp-loz/`
3. Test PWA functionality

## PWA Installation Instructions

### For iOS Devices:
1. Open the app in Safari
2. Tap the Share button (square with arrow up)
3. Scroll down and tap "Add to Home Screen"
4. Customize the name if desired
5. Tap "Add" in the top right

### For Android Devices:
1. Open the app in Chrome
2. Tap the three dots menu (⋮)
3. Select "Add to Home screen" or "Install app"
4. Confirm by tapping "Add" or "Install"

### For Desktop (Chrome/Edge):
1. Open the app in Chrome or Edge
2. Look for the install icon in the address bar
3. Click "Install" when prompted
4. The app will be added to your applications

## Features Included

### PWA Features:
- ✅ Offline functionality
- ✅ App-like experience
- ✅ Installable on mobile and desktop
- ✅ Responsive design
- ✅ Service worker caching
- ✅ Web app manifest

### App Features:
- 📅 Complete schedule with all sessions
- 👨‍🏫 Instructor information
- 📍 Location details with interactive maps
- 📱 Modern, mobile-first design
- 🎨 Smooth animations and transitions
- 🔍 Session details modal
- 📱 Touch-friendly interface

## Troubleshooting

### PWA Not Installing:
- Ensure HTTPS is enabled (GitHub Pages provides this automatically)
- Check that all manifest and service worker files are properly uploaded
- Verify icons are accessible and properly sized

### Maps Not Loading:
- The embedded Google Maps should work automatically
- If issues occur, check the iframe embed codes in the schedule data

### Offline Functionality:
- The service worker caches essential resources
- The app will work offline after the first visit
- Schedule data is embedded in the app for offline access

## Customization Options

### To Update Schedule:
1. Modify the `scheduleData` array in the index.html file
2. Update session information, times, instructors, and locations
3. Replace map embed codes as needed

### To Change Styling:
1. Modify CSS custom properties in the `:root` selector
2. Update colors, fonts, and spacing as desired
3. The design uses CSS Grid and Flexbox for responsive layouts

### To Add New Features:
1. The app is built with vanilla JavaScript for maximum compatibility
2. Additional features can be added to the existing codebase
3. Consider PWA best practices for offline functionality

## File Structure Summary
```
Repository Root/
├── index.html          (Main app - 15KB)
├── manifest.json       (PWA manifest - 2KB)
├── sw.js              (Service worker - 3KB)
├── icon-72.png        (72x72 icon)
├── icon-96.png        (96x96 icon)
├── icon-128.png       (128x128 icon)
├── icon-144.png       (144x144 icon)
├── icon-152.png       (152x152 icon)
├── icon-192.png       (192x192 icon)
├── icon-384.png       (384x384 icon)
└── icon-512.png       (512x512 icon)
```

## Additional Recommendations

1. **Test on Multiple Devices**: Verify the app works on iOS, Android, and desktop
2. **Monitor Performance**: Use Lighthouse to check PWA score and performance
3. **Update Content**: Keep schedule and instructor information current
4. **Backup Files**: Keep local copies of all files for future updates

Your modern skating camp PWA is ready for deployment! 🛼✨
