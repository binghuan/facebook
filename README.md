# Facebook Home Screen Shortcut

A progressive web app (PWA) that allows users to easily add Facebook as a shortcut to their home screen on Android and iOS devices.

## Features

- **Easy Installation**: Simple one-tap installation to home screen
- **Cross-Platform**: Works on both Android and iOS devices
- **Native-like Icons**: Includes optimized icons for different screen sizes and platforms
- **Auto-redirect**: Automatically redirects to Facebook after installation
- **Mobile Optimized**: Responsive design optimized for mobile browsers

## How It Works

This app provides a seamless way to add Facebook to your device's home screen:

1. **Visit the installation page** - Users access the pin2start.html page
2. **Display installation instructions** - Shows device-specific instructions for adding to home screen
3. **Install the shortcut** - Users follow the prompts to add the icon to their home screen
4. **Launch Facebook** - Once installed, tapping the icon redirects directly to Facebook

## Technical Details

### Files Structure

- `index.html` - Main app page with installation instructions and branding
- `pin2start.html` - Entry point that sets session storage and redirects to main page
- `main.js` - JavaScript logic for handling installation state and redirection
- `icons/` - Collection of app icons in various sizes for different platforms
- `images/` - UI elements (share and add-to-home icons)

### Icon Sizes Included

The app includes icons optimized for various platforms and screen densities:
- **iOS**: 60x60, 76x76, 120x120, 152x152
- **Android**: 48x48, 72x72, 96x96, 144x144, 192x192, 196x196
- **Desktop**: 16x16, 32x32, 64x64, 128x128, 256x256, 512x512, 1024x1024
- **Windows**: ICO format included

### Installation Process

1. **Session Management**: Uses `sessionStorage.PIN_TILE_STAY` to track installation state
2. **State Detection**: Checks if user is in "pin mode" or ready to launch
3. **Conditional Redirect**: Either shows installation page or redirects to Facebook

## Usage

### Quick Start

Scan the QR Code below to access the installation page:

<img src="pictures/QRCode.jpg" alt="QR Code for Facebook Home Screen Shortcut">

### Direct Link

Or visit directly: [http://binghuan.github.io/facebook/pin2start.html](http://binghuan.github.io/facebook/pin2start.html)

### Installation Steps

1. **Open the link** on your mobile device
2. **Tap the share button** (usually at the bottom of your browser)
3. **Select "Add to Home Screen"** from the menu
4. **Confirm** the installation
5. **Launch** the app from your home screen - it will redirect to Facebook

## Browser Support

- iOS Safari
- Android Chrome
- Android Firefox
- Other modern mobile browsers with PWA support

## Development

### Local Setup

1. Clone this repository
2. Serve the files using any web server (Python, Node.js, Apache, etc.)
3. Test on mobile devices or use browser developer tools with mobile emulation

### Customization

To adapt this for other websites:
- Update the redirect URL in `main.js` (line 32)
- Replace the icons in the `icons/` folder
- Modify the title and branding in `index.html`
- Update the QR code to point to your deployment URL
