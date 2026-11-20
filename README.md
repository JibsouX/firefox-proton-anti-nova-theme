# Firefox Proton Anti-Nova Theme

A faithful CSS theme and icon pack that restores Firefox's classic **Proton** interface and iconography on modern Firefox builds where the **Nova** redesign is enabled by default.

---

## About This Project

Mozilla's **Nova** redesign introduces pill-shaped buttons, wider corner radii, violet accent tints, translucent backgrounds, and redesigned icons across Firefox. As the `browser.nova.enabled` preference is phased out and Nova becomes mandatory, **Firefox Proton Anti-Nova Theme** provides a clean, self-contained way to keep the familiar **Proton** look and feel.

**What it does:**
- Restores the classic Proton visual language across the entire browser interface (`userChrome.css`).
- Replaces Nova's icons with the original Proton vector icons (`proton-icons.css` + `icons/`).
- Brings internal Firefox pages back in line with Proton's clean styling (`userContent.css`).
- Works purely through Firefox's built-in user stylesheets—no browser binaries or internal archives need to be modified.

---

## Preview

https://github.com/user-attachments/assets/ae886d5d-e59d-487f-9e87-dbf26a0b8484

---

## What's Covered

### Design System & Themes
- **Full Theme Support:** Works seamlessly with Light Mode, Dark Mode, System Auto, and Private Browsing windows.
- **Classic Proton Colors:** Replaces Nova's violet tints and pastel gradients with Proton's neutral surfaces and signature blue/cyan accents.
- **Balanced Proportions:** Reverts Nova's heavily rounded pill shapes and oversized popups back to Proton's tighter, more restrained corners, and restores square web viewport corners.
- **UI Densities & Platforms:** Designed and tested primarily on macOS, with support for Windows, Linux, and Normal, Compact, and Touch densities.

### Tabs, Tab Groups & Containers
- **Floating Tabs:** Restores Proton's detached floating active tab appearance, subtle drop shadow, and classic close button.
- **Tab Groups:** Brings back Proton's rounded rectangular group pills, inverted collapsed pills, continuous bottom underline, native color palette, and group editor swatches.
- **Container Tabs:** Preserves classic top container indicator lines on tabs and clean text-and-icon indicators in the address bar.
- **Hover Previews:** Restores compact Proton styling for both single-tab previews and tab group hover menus.

### Address Bar & Search
- **Classic Megabar:** Restores Proton's focused outline, clean expansion geometry, neutral drop shadow, and flat search engine switcher.
- **Results Dropdown:** Aligns the suggestions panel with Proton's top separator line, classic title/URL separator, selection highlights, and Proton-styled tab group and switch-to-tab badges.

### Complete Proton Icon Pack
- Includes a local set of pure Proton SVG icons covering navigation controls, toolbar buttons, sidebar toggles (left and right positions), tab strip actions, address bar controls, search sources, findbar buttons, and context/application menus.
- Dynamically adapts icon colors to your active theme while preserving colored states (such as bookmarked stars, active downloads, and security indicators).

### Menus, Chrome & Internal Pages
- **Browser Chrome:** Restores the classic Firefox Account banner in the application menu, Proton-styled context menus, Findbar, Sidebar splitters, Picture-in-Picture controls, and the labeled Private Browsing indicator.
- **Internal Pages:** Applies Proton styling to built-in pages such as Settings (`about:preferences`), Add-ons (`about:addons`), New Tab / Home (`about:newtab`, `about:home`), Firefox View, Private Browsing, Keyboard Shortcuts, and diagnostic pages—while intentionally leaving `about:blank`, Reader Mode, and Developer Tools untouched.

---

## Installation

1. **Enable custom stylesheets in Firefox:**
   - Open a new tab and go to `about:config`.
   - Accept the warning if prompted.
   - Search for `toolkit.legacyUserProfileCustomizations.stylesheets` and set it to **`true`**.

2. **Open your Firefox profile folder:**
   - Go to `about:support`.
   - Find the **Profile Folder** row and click **Open Folder** (or **Show in Finder** on macOS).

3. **Install the theme:**
   - Download or clone this repository (`firefox-proton-anti-nova-theme`).
   - Copy the entire `chrome/` folder into your Firefox profile folder.
   - *(If you already have a `chrome/` folder, back it up first before replacing or merging its contents.)*

4. **Restart Firefox:**
   - Fully quit and relaunch Firefox for all changes to take effect.

---

## Updating & Uninstalling

- **To update:** Replace the `chrome/` folder in your Firefox profile with the latest version from this repository and restart Firefox.
- **To uninstall:** Delete (or rename) the `chrome/` folder inside your profile directory and restart Firefox.

---

## Notes & License

- Built against Firefox's native Proton design tokens and SVG assets.
- Original Firefox icons and derived styles are subject to the **Mozilla Public License 2.0 (MPL-2.0)**.
