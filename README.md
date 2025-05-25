# Vivaldi Auto-Hide Bookmark Bar

A sleek CSS modification for Vivaldi browser that creates an auto-hiding bookmark bar with smooth animations and hover effects.

## ✨ Features

- **Auto-hide functionality**: Bookmark bar stays hidden until you need it
- **Smooth animations**: Elegant slide-in/out transitions with customizable timing
- **Smart hover detection**: Shows on header, tab strip, or bookmark bar hover
- **Delayed hiding**: 2-second delay before hiding to prevent accidental disappearance
- **Clean tab design**: Centered favicons with hidden close buttons and titles
- **High z-index**: Ensures bookmark bar appears above all other UI elements

## 🎥 Demo

![Screenshot](/screenshot.png)
<div align="center">
  <img src="demo.gif" alt="Demo">
</div>

The bookmark bar will:
1. Stay hidden by default for a clean browsing experience
2. Smoothly slide down when you hover over the browser header or tabs
3. Remain visible while you're interacting with it
4. Hide automatically after 2 seconds when you stop hovering

## 📦 Installation

1. **Enable CSS modifications in Vivaldi**:
   - Go to `vivaldi://experiments/`
   - Enable "Allow for using CSS modifications"
   - Restart Vivaldi

2. **Locate your Vivaldi profile folder**:
   - **Windows**: `%LOCALAPPDATA%\Vivaldi\User Data\Default`
   - **macOS**: `~/Library/Application Support/Vivaldi/Default`
   - **Linux**: `~/.config/vivaldi/Default`

3. **Create the custom CSS file**:
   - Create a file named `vivaldi.css` in your profile folder
   - Copy the CSS code from this repository into the file
   - Save and restart Vivaldi

## 🎨 Customization

You can easily customize the behavior by modifying the CSS variables at the top of the file:

```css
:root {
  --vivaldi-bookmark-bar-height: 30px;     /* Height of the bookmark bar */
  --vivaldi-header-height: 34px;           /* Adjust based on your UI */
  --bookmark-bar-hide-delay: 2s;           /* Delay before hiding (in seconds) */
  --bookmark-bar-animation-duration: 0.2s; /* Animation speed */
  --bookmark-bar-shadow: 0 2px 5px rgba(0, 0, 0, 0.15); /* Drop shadow */
  --bookmark-bar-z-index: 10000;           /* Stacking order */
}
```

### Popular Customizations

**Faster animations**:
```css
--bookmark-bar-animation-duration: 0.1s;
```

**Longer delay before hiding**:
```css
--bookmark-bar-hide-delay: 5s;
```

**No shadow**:
```css
--bookmark-bar-shadow: none;
```

## 🔧 Troubleshooting

### Bookmark bar appears behind other elements
- Increase the z-index value:
  ```css
  --bookmark-bar-z-index: 99999;
  ```

### Delay not working properly
- Make sure you're using the latest version of the CSS
- Try disabling other Vivaldi modifications temporarily

### Animation feels choppy
- Reduce the animation duration:
  ```css
  --bookmark-bar-animation-duration: 0.1s;
  ```

### Bookmark bar height issues
- Adjust the height variable to match your bookmark bar:
  ```css
  --vivaldi-bookmark-bar-height: 35px;
  ```

## 🤝 Contributing

Found a bug or have a suggestion? Feel free to:
- Open an issue
- Submit a pull request
- Share your customizations

## 📝 License

This project is licensed under the MIT License - feel free to use and modify as needed.

## 🙏 Acknowledgments

- Thanks to the Vivaldi community for inspiration and testing
- Built for Vivaldi browser users who love clean, minimal interfaces

---

**Note**: This modification requires Vivaldi's experimental CSS feature to be enabled. Use at your own discretion and always backup your profile before making modifications.
