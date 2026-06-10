# 🎨 Color Dictation - Teachable Machine Website

A beautiful, responsive website showcasing real-time image classification using **Teachable Machine** with two different implementations.

## Features

✨ **Two Implementation Options:**
- **TensorFlow.js** - High-performance, detailed confidence scores
- **p5.js + ml5.js** - Creative coding, beginner-friendly

🎯 **Key Features:**
- Real-time webcam classification
- Live confidence scores
- Responsive design (mobile-friendly)
- Professional UI with smooth animations
- Privacy-first (all processing in browser)
- One-click start/stop controls

## Getting Started

### 1. **Open the Website**
Simply open `index.html` in your web browser:
```bash
# On Windows, double-click the file, or
# Open in VS Code and use Live Server extension
```

### 2. **Allow Webcam Access**
When prompted, allow the browser to access your webcam.

### 3. **Start Classification**
- Click the **"Start Webcam"** button
- Point your camera at different objects/colors
- Watch real-time predictions appear

## Two Implementations

### 🔧 TensorFlow.js Implementation
- Uses official Teachable Machine library
- Provides detailed confidence percentages
- Faster inference
- Better for accuracy-critical applications

**Tab 1:** Click the "TensorFlow.js" tab to use this implementation.

### 🎨 p5.js + ml5.js Implementation  
- Uses p5.js for drawing and ml5.js for ML
- Great for artistic projects
- Simplified API
- Easier to extend with creative code

**Tab 2:** Click the "p5.js + ml5.js" tab to use this implementation.

## Model Information

The website uses a pre-trained Teachable Machine model:
```
Model URL: https://teachablemachine.withgoogle.com/models/oSzr7R5d3/
```

**To use your own model:**
1. Go to [Teachable Machine](https://teachablemachine.withgoogle.com/)
2. Train your custom image classification model
3. Export the model URL
4. Replace the `MODEL_URL` in `index.html` (line 281)

## Customization

### Change the Model
```javascript
// In index.html, change this line:
const MODEL_URL = "https://teachablemachine.withgoogle.com/models/YOUR_MODEL_ID/";
```

### Adjust Webcam Size
In the `initTFJS()` function:
```javascript
tfjsWebcam = new tmImage.Webcam(300, 300, flip); // width, height, flip
```

### Modify Colors/Styling
Edit the CSS in the `<style>` section:
```css
/* Change the gradient colors */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

## Browser Compatibility

✅ Chrome/Edge 90+
✅ Firefox 88+
✅ Safari 14+
✅ Mobile browsers (iOS Safari, Chrome Mobile)

## Requirements

- **Modern web browser** (with WebGL support)
- **Webcam** access permission
- **Internet connection** (to load ML models from CDN)

## Files Included

```
teachable/
├── index.html          # Main website (all-in-one)
└── README.md           # This file
```

## What You Can Classify

- 🎨 **Colors** - Red, blue, green, etc.
- 🐕 **Objects** - Dogs, cats, plants, etc.
- 🤟 **Gestures** - Hand signs, poses, etc.
- 📝 **Anything** - Train a custom Teachable Machine model!

## Libraries Used

- **TensorFlow.js** - Machine learning in JavaScript
- **Teachable Machine** - Easy ML model creation
- **p5.js** - Creative coding library
- **ml5.js** - ML5 wrapper for TensorFlow.js
- **HTML5 Canvas** - Video rendering

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Tab` | Switch between implementations |
| `Click button` | Start/stop webcam |

## Troubleshooting

### Webcam not showing?
- Check if browser has webcam permission
- Try refreshing the page
- Use a different browser

### Model loading slowly?
- Check internet connection
- Clear browser cache
- Try again after a few seconds

### Classification inaccurate?
- Make sure proper lighting
- Get closer/further from camera
- Train a custom model with your specific use case

## Future Enhancements

- [ ] Download classification history
- [ ] Statistics dashboard
- [ ] Custom model upload
- [ ] Voice feedback
- [ ] Multi-model support
- [ ] Export results to CSV

## License

This project uses Google's Teachable Machine - see their [terms](https://teachablemachine.withgoogle.com/).

## Support

For issues with Teachable Machine models, visit:
- [Teachable Machine Community](https://github.com/googlecreativelab/teachablemachine-community)
- [ml5.js Documentation](https://learn.ml5js.org/)
- [TensorFlow.js Documentation](https://www.tensorflow.org/js)

---

**Happy classifying! 🚀**
