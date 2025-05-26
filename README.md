# Mobile AR Event Experience - Image Marker Video Trigger

A cross-platform mobile web application for event attendees to scan a custom PNG marker image with their smartphones and automatically trigger video content playback.

## 🎯 Project Overview

This mobile-optimized web application allows event guests to:
1. Access the experience via any mobile browser (iOS/Android)
2. Scan a pre-designed PNG marker image using their phone camera
3. Automatically trigger and play an MP4 video when the marker is detected
4. Enjoy a seamless AR experience without downloading any apps

## ✨ Features

- **Cross-Platform Mobile Support**: Works on iOS Safari and Android Chrome/Firefox
- **Image Marker Detection**: Uses AR.js for robust PNG marker recognition
- **Auto-Play Video**: Seamless MP4 video playback on marker detection
- **No App Installation Required**: Pure web-based solution
- **Event-Ready Design**: Optimized for event environments and varying lighting
- **Responsive Mobile UI**: Touch-friendly interface for mobile devices

## 🛠 Tech Stack

- **HTML5** - Structure and mobile viewport optimization
- **CSS3** - Mobile-responsive design and video overlays
- **JavaScript (ES6+)** - Camera handling and video control logic
- **AR.js** - WebRTC-based AR marker detection
- **A-Frame** - 3D/AR scene management
- **WebRTC** - Camera access for marker scanning

## 📱 Mobile Browser Compatibility

| Platform | Browser | Status |
|----------|---------|--------|
| iOS 13+ | Safari | ✅ Full Support |
| iOS 13+ | Chrome/Firefox | ✅ Full Support |
| Android 8+ | Chrome | ✅ Full Support |
| Android 8+ | Firefox | ✅ Full Support |
| Android 8+ | Samsung Browser | ✅ Full Support |

## 🚀 Quick Setup for Events

1. **Deploy the web app** to your hosting platform
2. **Upload your custom PNG marker** to `/assets/markers/`
3. **Upload your event MP4 video** to `/assets/videos/`
4. **Generate QR code** linking to your deployed URL
5. **Share QR code** with event attendees

## 📋 Event Requirements

### Essential Files Needed:
- **Custom PNG Marker Image** (recommended: high contrast, unique pattern)
- **Event MP4 Video** (optimized for mobile: 1080p max, H.264 codec)
- **Hosting Platform** (Netlify, Vercel, GitHub Pages, or custom server)

### Technical Requirements:
- HTTPS hosting (required for camera access)
- Mobile-optimized server with video streaming support
- Fast CDN for optimal video loading

## 🔧 Development & Testing

### Local Development:
```bash
# Install a local HTTPS server (required for camera access)
npm install -g http-server
# or
npm install -g live-server

# Serve with HTTPS (required for mobile camera)
http-server -S -C cert.pem -K key.pem -p 8080
# or use ngrok for HTTPS tunnel
ngrok http 8080
```

### Mobile Testing:
1. **Test on actual devices** - Camera behavior varies between browsers
2. **Verify auto-play policies** - Some browsers require user interaction
3. **Check marker detection range** - Test in various lighting conditions
4. **Validate video loading** - Ensure smooth playback on mobile networks

## 📐 Marker Design Guidelines

For optimal detection on mobile devices:
- **Size**: Minimum 200x200px, recommended 500x500px
- **Contrast**: High contrast black/white elements
- **Complexity**: Detailed enough to be unique, simple enough for mobile cameras
- **Border**: Include clear white border around the marker
- **Format**: PNG with transparent background support

## 🎬 Video Optimization

Recommended MP4 settings for mobile:
- **Resolution**: 720p-1080p maximum
- **Codec**: H.264 (baseline profile for compatibility)
- **Bitrate**: 1-3 Mbps for mobile networks
- **Duration**: Keep under 30 seconds for optimal loading
- **Audio**: AAC codec, consider muted auto-play compliance

## 🌐 Deployment Options

### Recommended Platforms:
- **Netlify**: Easy deployment with HTTPS
- **Vercel**: Optimized for mobile performance
- **GitHub Pages**: Free hosting with custom domains
- **AWS S3 + CloudFront**: Scalable for large events

### Performance Considerations:
- Enable gzip compression for faster loading
- Use CDN for video assets
- Implement lazy loading for non-critical resources
- Optimize images and compress videos

## 🔒 Privacy & Permissions

- Camera access required (users will see browser permission prompt)
- No video recording - only real-time marker detection
- No personal data stored or transmitted
- Event attendee privacy compliant

## 📞 Event Support

### For Event Organizers:
- Test the experience before your event
- Provide clear instructions to attendees
- Have backup QR codes ready
- Consider lighting conditions at venue

### Troubleshooting:
- Ensure attendees allow camera permissions
- Verify HTTPS connection for camera access
- Test marker visibility in event lighting
- Have technical support contact available

## 📄 License

MIT License - Perfect for event and commercial use

---

**Ready to create an unforgettable event experience? Start by uploading your marker image and video content!** 