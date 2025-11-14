# Bookmarks

A beautiful, standalone HTML bookmark manager with category filtering and search functionality. No server required—just open the HTML file in your browser and start organizing your favorite links.

## ✨ Features

- **Category-based Organization**: Organize bookmarks into categories (Documentation, News, Training Resources, etc.)
- **Real-time Search**: Quickly find bookmarks by name or description
- **Clean, Modern UI**: Gradient backgrounds, smooth animations, and responsive design
- **Zero Dependencies**: Pure HTML, CSS, and JavaScript—no build tools or frameworks needed
- **Fully Customizable**: Easy to add, edit, or remove bookmarks directly in the HTML

## 🚀 Quick Start

1. Download or clone this repository
2. Open `bookmarks.html` in your web browser
3. Start using your personalized bookmark manager!

That's it! No installation, no setup, no dependencies.

## 📖 Usage

### Viewing Bookmarks

- **View All**: Click the "All" button in the category bar to see all bookmarks
- **Filter by Category**: Click any category button (Documentation, News, Training Resources) to show only that category
- **Search**: Type in the search box to filter bookmarks by name or description in real-time

### Adding Bookmarks

To add a new bookmark, add a new `bookmark-item` div inside the appropriate category section:

```html
<div class="bookmark-item">
    <a class="bookmark-name" href="https://example.com" target="_blank">Example Site</a>
    <div class="bookmark-description">A brief description of what this site is about.</div>
</div>
```

### Adding Categories

To add a new category:

1. Add a category button in the category bar:
```html
<div class="category-item" onclick="showOnlyCategory('Your Category', this)">Your Category</div>
```

2. Create a new bookmark list section:
```html
<div id="Your Category" class="bookmark-list">
    <!-- Your bookmarks go here -->
</div>
```

### Editing Bookmarks

Simply edit the HTML directly:
- Change the `href` attribute to update the URL
- Modify the link text to change the bookmark name
- Update the description text inside the `bookmark-description` div

## 🎨 Customization

### Changing Colors

The color scheme can be customized by modifying the CSS variables and gradient values in the `<style>` section. Key color values to look for:
- Primary blue: `#2d89ef`, `#0078d4`
- Gradient colors: `#6ecefb`, `#73e8f4`
- Background gradients: `#f7fafc`, `#e0f7fa`

### Adjusting Layout

- Modify `.container` max-width to change the overall width
- Adjust padding and margins in `.bookmark-item` for spacing
- Change border-radius values for rounded corners

## 🛠️ Technologies Used

- **HTML5**: Structure and content
- **CSS3**: Styling with gradients, transitions, and responsive design
- **JavaScript**: Category filtering and search functionality

## 📝 Notes

- All links open in a new tab (`target="_blank"`)
- The search function searches both bookmark names and descriptions
- Categories can be hidden/shown dynamically via JavaScript
- The page uses modern CSS features (gradients, transitions) supported by all major browsers

## 💡 Tips

- Bookmark this page in your browser for easy access
- You can export this HTML file and use it on any device
- Consider hosting this file on a local web server or cloud storage for access from multiple devices
- Keep your categories organized and use descriptive bookmark names for better search results

## 📄 License

This project is open source and available for personal use. Feel free to customize it to fit your needs!

---

Made with ❤️ for better bookmark organization
