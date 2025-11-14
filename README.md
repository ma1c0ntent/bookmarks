# Bookmarks

[![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)](CHANGELOG.md)

A beautiful, standalone HTML bookmark manager with category filtering, tag-based organization, real-time search with highlighting, and sorting options. No server required—just open the HTML file in your browser and start organizing your favorite links.

## ✨ Features

- **Category-based Organization**: Organize bookmarks into categories (Documentation, News, Training Resources, etc.)
- **Real-time Search**: Quickly find bookmarks by name, description, or tags with search term highlighting
- **Tag System**: Add tags to bookmarks for more granular filtering and organization
- **Sorting Options**: Sort bookmarks by name (A-Z, Z-A), category, or original order
- **Bookmark Counts**: See how many bookmarks are in each category, updated dynamically based on filters
- **Keyboard Shortcuts**: Press Esc to clear the search input
- **Search Highlighting**: Search terms are highlighted in yellow within bookmark names and descriptions
- **Clean, Modern UI**: Gradient backgrounds, smooth animations, and responsive design with improved contrast
- **Zero Dependencies**: Pure HTML, CSS, and JavaScript—no build tools or frameworks needed
- **Fully Customizable**: Easy to add, edit, or remove bookmarks directly in the HTML
- **Persistent Preferences**: Sort order is saved and restored automatically using localStorage

## 🚀 Quick Start

1. Download or clone this repository
2. Open `bookmarks.html` in your web browser
3. Start using your personalized bookmark manager!

That's it! No installation, no setup, no dependencies.

## 📖 Usage

### Viewing Bookmarks

- **View All**: Click the "All" button in the category bar to see all bookmarks
- **Filter by Category**: Click any category button (Documentation, News, Training Resources) to show only that category
- **Search**: Type in the search box to filter bookmarks by name, description, or tags in real-time
  - Search terms are highlighted in yellow within matching bookmarks
  - Press **Esc** to clear the search input
- **Filter by Tags**: Click on any tag (#tag) on a bookmark to filter by that tag
  - Click "Clear Filter" to remove the tag filter
- **Sort Bookmarks**: Use the "Sort by" dropdown to sort bookmarks:
  - **Default (Original Order)**: Restores the original order
  - **Name (A-Z)**: Alphabetical order
  - **Name (Z-A)**: Reverse alphabetical order
  - **Category**: Groups bookmarks by category
- **Bookmark Counts**: See the number of bookmarks in each category displayed as badges

### Adding Bookmarks

To add a new bookmark, add a new `bookmark-item` div inside the appropriate category section:

```html
<div class="bookmark-item">
    <a class="bookmark-name" href="https://example.com" target="_blank">Example Site</a>
    <div class="bookmark-description">A brief description of what this site is about.</div>
    <div class="bookmark-tags">
        <span class="tag" onclick="filterByTag('programming', this)">#programming</span>
        <span class="tag" onclick="filterByTag('tutorial', this)">#tutorial</span>
    </div>
</div>
```

**Note**: Tags are optional but recommended for better organization and filtering.

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
- Add, remove, or modify tags in the `bookmark-tags` div
- Change tag names to match your organization system

## 🎨 Customization

### Changing Colors

The color scheme can be customized by modifying the CSS variables and gradient values in the `<style>` section. Key color values to look for:
- Primary blue: `#2d89ef`, `#0078d4`
- Navbar gradient: `#1a5490`, `#2d5aa0` (darker for better contrast)
- Background gradients: `#f7fafc`, `#e0f7fa`
- Highlight color: `#fff176` (yellow for search term highlighting)
- Category button colors: `#005a9e` (hover), `#004578` (active)

### Adjusting Layout

- Modify `.container` max-width to change the overall width
- Adjust padding and margins in `.bookmark-item` for spacing
- Change border-radius values for rounded corners

## 🛠️ Technologies Used

- **HTML5**: Structure and content
- **CSS3**: Styling with gradients, transitions, and responsive design
- **JavaScript**: Category filtering, tag filtering, search functionality, sorting, and highlighting
- **localStorage**: Persisting user preferences (sort order)

## 📝 Notes

- All links open in a new tab (`target="_blank"`)
- The search function searches bookmark names, descriptions, and tags
- Search terms are highlighted in yellow for easy identification
- Categories can be hidden/shown dynamically via JavaScript
- Tag filters work in combination with category filters and search
- Sort preferences are saved automatically and persist across page reloads
- Bookmark counts update dynamically based on active filters
- Browser autocomplete is disabled on the search input for a cleaner experience
- The page uses modern CSS features (gradients, transitions) supported by all major browsers

## 💡 Tips

- Bookmark this page in your browser for easy access
- You can export this HTML file and use it on any device
- Consider hosting this file on a local web server or cloud storage for access from multiple devices
- Keep your categories organized and use descriptive bookmark names for better search results
- Use tags consistently across bookmarks for effective filtering
- Combine category filters, tag filters, and search for precise bookmark discovery
- Press Esc to quickly clear the search input
- Sort by category to see all bookmarks grouped by their category
- Bookmark counts help you see how many results match your current filters

## 📝 Changelog

See [CHANGELOG.md](CHANGELOG.md) for a list of changes and version history.

## 📄 License

This project is open source and available for personal use. Feel free to customize it to fit your needs!

---

Made with ❤️ for better bookmark organization
