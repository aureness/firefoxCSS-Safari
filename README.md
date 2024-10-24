# Firefox Safari theme

<picture width="50">
  <source media="(prefers-color-scheme: dark)" srcset="./screenshots/dark.png?raw=true">
  <source media="(prefers-color-scheme: light)" srcset="./screenshots/light.png?raw=true">
  <img alt="Screenshot of the Firefox browser with my theme">
</picture>


Inspired by Apple Safari design. I've tried to mimic as close as I can (and as I want).

Some styles are based on the [vinceliuice/WhiteSur-firefox-theme](https://github.com/vinceliuice/WhiteSur-firefox-theme/). 
I have added you to the LICENSE and mentioned here :)

## Installation
Add this line yo your `userChrome.css`
```css
@import "safari/theme.css";
```

If you don't know what is `userChrome.css` read the manual: https://www.userchrome.org/

Go to `about:config` in Firefox.
Search for `toolkit.legacyUserProfileCustomizations.stylesheets` and set it to `true`.

Customize your Toolbar: move buttons around.

Add some plugins like: https://addons.mozilla.org/en-US/firefox/addon/reload-in-address-bar/

## Customization

You can comment out (or comment in!) lines from the `safari/theme.css` file in the `/* OPTIONS */` section.

For example: if you don't like how tabbar is hidden when there is only one tab, comment this line:
```css
/* @import "parts/hide-single-tab.css" */
```
All options:
```css
/* OPTIONS */
@import "parts/sticky-tabs.css"; /* active tab will be always visible at the edge of the window  */
@import "parts/drag-window-toolbar.css"; /* dragging by clicking toolbar */
@import "parts/hide-menu-btn.css"; /* hide menu button and use global menu instead */
@import "parts/hide-single-tab.css"; /* hide tabbar if only one page is opened */
@import "parts/tabs-fill-tabbar.css"; /* wide tabs filling all tabbar, no max-width */
@import "parts/tab-close-btn-left.css"; /* show close tab btn at left */
@import "parts/tab-close-btn-only-active-tab.css"; /* always show close btn only on active tab, and on hover on others */
@import "parts/fade-tab-title-inactive-wnd.css"; /* tab title if fade in grey if window is not focused */
@import "parts/custom-icons.css"; /* custom icons in macOS style */
@import "parts/hide-all-tabs-btn.css"; /* hide All tabs button with drop down menu */
```
