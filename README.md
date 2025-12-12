# YouTube Subscription Feed - List View

Restore the classic list view for YouTube subscriptions feed that YouTube removed.

<img width="1822" height="879" alt="image" src="https://github.com/user-attachments/assets/5bea21d6-55c1-4230-aa59-f5257ad0a6cd" />


## Installation

### 1. Install Stylus Extension

- **Chrome**: [Stylus - Chrome Web Store](https://chromewebstore.google.com/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne)
- **Firefox**: [Stylus - Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/styl-us/)

### 2. Apply the Style

1. Click the Stylus extension icon in your browser toolbar
2. Click "Manage" or "Write new style"
3. Copy the CSS from `youtube-list-view.css`
4. Paste it into the style editor
5. Set "Applies to" → "URLs starting with" → `https://www.youtube.com/feed/subscriptions`
6. Save the style

<img width="1910" height="910" alt="image" src="https://github.com/user-attachments/assets/c6391fe9-715f-464a-bd62-3ec534d27d70" />


## Features

- ✅ Classic horizontal list layout
- ✅ Larger thumbnails with proper aspect ratio
- ✅ Hover effects for better UX
- ✅ Clean separators between videos
- ✅ Responsive design for different screen sizes
- ✅ Hides Shorts section (optional)

## Customization

Edit the CSS variables at the top of the file:

```css
:root {
    --thumbnail-width: 246px;
    --thumbnail-height: 138px;
    --content-gap: 16px;
    --title-size: 15px;
    --meta-size: 13px;
}
```

## Keep Shorts Visible

Remove or comment out this section:

```css
ytd-rich-section-renderer #dismissible {
    display: none;
}
```

## Issues

If the style doesn't work:
- Make sure you're on `youtube.com/feed/subscriptions`
- Try refreshing the page
- Check that Stylus is enabled for YouTube
- Verify the style is active in Stylus manager

## License

MIT
