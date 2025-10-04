## Author

**HennessyAbhi**  
GitHub: [https://github.com/HennessyAbhi](https://github.com/HennessyAbhi)

# Google Maps Embedded Code Examples

This repository contains examples of how to embed Google Maps into your web pages using iframe elements. The examples demonstrate different ways to display maps, directions, and search results.

## Files

- `google-map.html` - Contains three different examples of embedded Google Maps

## Examples Included

### Example 1: Basic Location Map
```html
<iframe
  width="600"
  height="450"
  style="border:0"
  loading="lazy"
  allowfullscreen
  referrerpolicy="no-referrer-when-downgrade"
  src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3430.338073289889!2d75.8572743151322!3d30.90096568156359!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x391a832b2e2e7b1d%3A0x6e7e0e92ce40938e!2sLudhiana%2C%20Punjab%2C%20India!5e0!3m2!1sen!2sza!4v1680000000000!5m2!1sen!2sza">
</iframe>
```
**What it does:** Displays a map centered on Ludhiana, Punjab, India.

### Example 2: Directions Map
```html
<iframe
  width="600"
  height="450"
  style="border:0"
  loading="lazy"
  allowfullscreen
  referrerpolicy="no-referrer-when-downgrade"
  src="https://www.google.com/maps/embed?pb=!1m28!1m12!1m3!1d14013.964024052499!2d77.216721!3d28.644800!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!4m13!3e0!4m5!1s0x390cfd1e6b1e1b1b%3Ax6e7e0e92ce40938e!2sDelhi!3m2!1d28.704060!2d77.102493!4m5!1s0x391a832b2e2e7b1d%3A0x6e7e0e92ce40938e!2sLudhiana%2C%20Punjab%2C%20India!3m2!1d30.9009657!2d75.8572743!5e0!3m2!1sen!2sza!4v1680000000001!5m2!1sen!2sza">
</iframe>
```
**What it does:** Shows driving directions from Delhi to Ludhiana.

### Example 3: Search Results Map
```html
<iframe
  width="600"
  height="450"
  style="border:0"
  loading="lazy"
  allowfullscreen
  referrerpolicy="no-referrer-when-downgrade"
  src="https://www.google.com/maps/embed/v1/search?key=YOUR_API_KEY&q=restaurants+near+Ludhiana+Punjab+India">
</iframe>
```
**What it does:** Displays search results for restaurants near Ludhiana (requires Google Maps API key).

## How to Use

### Method 1: Copy and Paste
1. Open `google-map.html` in a text editor
2. Copy the iframe code you want to use
3. Paste it into your HTML page where you want the map to appear
4. Adjust the `width` and `height` attributes as needed

### Method 2: Generate Your Own Embed Code
1. Go to [Google Maps](https://maps.google.com)
2. Search for the location you want to display
3. Click the "Share" button
4. Select "Embed a map"
5. Copy the provided iframe code
6. Paste it into your HTML page

## Customization Options

### Size and Styling
- **Width/Height**: Adjust the `width` and `height` attributes to fit your layout
- **Border**: Remove the border by setting `style="border:0"` (already included)
- **Responsive**: Add CSS to make the map responsive:
  ```css
  .map-container {
    position: relative;
    width: 100%;
    height: 0;
    padding-bottom: 56.25%; /* 16:9 aspect ratio */
  }
  .map-container iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
  ```

### Map Features
- **Zoom Level**: Modify the zoom parameter in the URL (higher numbers = more zoomed in)
- **Map Type**: Change between roadmap, satellite, hybrid, or terrain views
- **Language**: Modify the language parameters (`1sen!2sza` = English/South Africa)

## API Key Setup (for Search Maps)

Example 3 requires a Google Maps API key:

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project or select an existing one
3. Enable the "Maps Embed API"
4. Create credentials (API key)
5. Replace `YOUR_API_KEY` in Example 3 with your actual API key

## Browser Compatibility

These embedded maps work in all modern browsers:
- Chrome
- Firefox
- Safari
- Edge
- Internet Explorer 11+

## Privacy and Terms

- Maps are loaded from Google's servers
- Usage is subject to Google's Terms of Service
- For commercial use, check Google's licensing requirements
- Consider privacy implications when embedding maps

## Troubleshooting

**Map not displaying?**
- Check your internet connection
- Verify the iframe src URL is correct
- Ensure no ad blockers are blocking the map
- Check browser console for errors

**API key issues?**
- Verify your API key is correct
- Ensure the Maps Embed API is enabled
- Check your API key restrictions
- Monitor your API usage quotas

## License

This code is provided as-is for educational and reference purposes. Please comply with Google's Terms of Service when using embedded maps.
