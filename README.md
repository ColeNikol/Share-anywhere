# Share-anywhere
Share button to share your web page anywhere

How to Use the Share-anywhere

Easy Integration for Any Website
This universal share solution makes it simple to add comprehensive sharing capabilities to any webpage with just a few lines of code.

What You Get
One-click sharing to 20+ social platforms

Smart detection of page title, description and image

Modern interface with category filters and search

Lightweight - no external dependencies

Mobile-friendly responsive design

Installation Instructions
1. Add the Share Button
Embed this code anywhere on your page where you want the share button to appear:

html
<div id="universal-share-button" style="...">
  <svg>...</svg>
  Share
</div>

<script>
// [The full share button code from share-button.html]
</script>
2. Host the Share Panel
Upload the share-panel.html file to your server. The button will automatically open this panel when clicked.

How It Works
Automatically Detects:

Current page URL

Page title (from <title> tag or Open Graph)

Description (from meta tags)

Featured image (prioritizes Open Graph/Twitter cards)

When Clicked:

Opens a clean share panel in a popup window

Shows preview of what will be shared

Organizes platforms by category (Social, Messaging, etc.)

User Experience:

Filter platforms by category tabs

Search for specific platforms

Click any platform to open its native share dialog

Customization Options
Styling the Button
You can easily customize the button's appearance by modifying the inline styles:

html
<div id="universal-share-button" style="
  background: #yourcolor;
  color: #yourtextcolor;
  /* Add other custom styles */
">
Adding More Platforms
To add additional sharing options, edit the socialPlatforms array in share-panel.html following the same format:

javascript
{
  name: 'PlatformName',
  color: '#hexcolor',
  category: 'categoryname',
  url: (u,t,d,i) => `share-url-template`
}
Best Practices
Place the button where users expect sharing options (near content)

Test on both desktop and mobile devices

Verify your page has proper Open Graph meta tags for best results

For high-traffic sites, consider hosting the panel on a CDN

Support
This solution works in all modern browsers and requires no special server-side configuration. The share panel will automatically adapt to the content being shared from each page.
