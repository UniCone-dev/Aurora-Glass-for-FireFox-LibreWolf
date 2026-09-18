# Aurora Glass — macOS × Edge New Tab

A Windows-Start-Menu-layout new tab page, restyled with a **macOS vibrancy + Microsoft
Edge Aurora** visual language: traffic-light window controls, squircle app icons, a
floating magnifying dock, frosted glass everywhere, spring-based motion, and now a
second full theme — **Sifiomini** — plus six interchangeable shortcut-icon styles.
100% local, open-source, no tracking, no analytics, no accounts. Everything is saved
directly inside your browser's local storage.

# Themes

Settings → Appearance → **Theme** lets you switch between two full looks, live:

- **Classic** — the original launcher panel: search bar up top, AI row, folders,
  and a floating dock at the bottom.
- **Sifiomini** — a calmer, hero-first layout inspired by Edge's own start
  page: a soft glowing orb, a short greeting, and one big centered search pill,
  with your pinned apps laid out underneath as quick-link tiles. The floating
  dock, wallpaper, dark/light mode, glass blur/opacity, and custom CSS all keep
  working exactly the same underneath either theme — only the panel layout changes.

# Shortcut styles

Independent of the theme, Settings → Appearance → **Shortcut style** changes how
every app/folder icon is drawn, everywhere in the UI (panel tiles, folders, the
dock). Six options:

1. **Square** — flat rounded-rectangle icons (classic Fluent).
2. **iOS** — a pronounced squircle, closer to iOS/iPadOS app icons.
3. **Card** — each shortcut sits in its own bordered glass card with the icon on
   top and the label inside, matching Edge's "Quick links" row.
4. **Circle** — fully round icons.
5. **Dock** — the default macOS-Dock-style rounded square with drop shadow
   (respects the separate "Squircle app icons" toggle for its exact curve).
6. **Minimal** — no background or shadow on the icon at all, just a flat glyph.

# What changed from the original Aurora Glass

- **Traffic-light buttons** — every panel's close button is now red/yellow/green,
  macOS-style (toggle back to a plain ✕ in Settings → Appearance).
- **Squircle icons** — app tiles, folder icons, and taskbar icons use a soft
  superellipse ("squircle") shape instead of a plain rounded square (Dock shortcut
  style only — see Shortcut styles above for five more options).
- **Floating dock** — the taskbar is now a centered, floating, rounded pill (like the
  macOS Dock) instead of an edge-to-edge Windows bar, with a hover-to-magnify effect.
- **Premium vibrancy glass** — panels use a stronger, saturated backdrop blur with an
  inner highlight, closer to macOS's frosted materials than the original flat glass.
- **Spring animations** — panels, tiles, and dock icons open and bounce with a
  spring easing curve instead of a linear/ease fade.
- **Edge Aurora wallpaper** — the default background is a soft mint/blue/green glow
  gradient inspired by Edge's own onboarding screen, plus new gradient presets.
- **Sifiomini theme** — an alternate, hero-first panel layout (see above).
- **Six shortcut styles** — Square / iOS / Card / Circle / Dock / Minimal (see above).
- **New Appearance settings**: a second accent color (so buttons render as a
  blue→green gradient like the Edge logo), a panel blur-intensity slider, on/off
  switches for traffic lights / dock magnify / squircle icons, and the theme +
  shortcut-style pickers — so you can dial the look back toward classic Fluent if
  you prefer, or push it all the way toward Sifiomini.
- **Home page support** — the same page can now also open as your browser's home
  page, not just the new-tab page (Firefox/LibreWolf will ask you to confirm this
  once, right after installing).

Everything else — the local AI row, folders, weather, taskbar pinning, CSS overrides,
export/import, Google sign-in (optional, bring-your-own OAuth Client ID) — works
exactly as before, under both themes and all six shortcut styles.

# Key Features

    Floating OS-style dock (bottom of screen, always visible): The Start button and pinned apps are centered in a floating glass pill, just like the macOS Dock — pin any AI/folder app using the "+" button or create a new custom app, and hover to see it magnify. The right tray shows a weather icon next to the temperature and clock, alongside a language switcher.

    Two themes (Classic / Sifiomini) and six shortcut-icon styles (Square / iOS / Card / Circle / Dock / Minimal), switchable live from Settings → Appearance.

    3 languages, fully translated: English (formal, default), Русский (Russian), Français (French). Every settings tab, button, hint, and placeholder is translated (excluding the search bar). Switch languages instantly via the top-right globe icon 🌐 or via Settings → Layout — clock and date formats automatically update to match the selected language.

    Custom app icons: Instead of just letters or emojis, you can upload your own image for any app (AI, folder, taskbar) via the "Custom icon image" option when editing an app.

    Fully customizable panel size and glass: Adjust width, max-height, scale, corner roundness, and blur intensity, with live previews (Settings → Layout / Appearance).

    Profile: Set your name and display picture (saved locally on your device). Optionally, you can connect your Google account by providing your own Google OAuth Client ID (Settings → Profile). Since this extension does not use any shared or centralized authentication server, Google login will only function after you enter your Client ID (instructions provided below).

    Search bar (top): A frosted Spotlight-style pill. Entering a link/URL opens it directly; entering regular text initiates a privacy-focused web search (default: DuckDuckGo — can be changed to Startpage, Brave, Google, or Bing).
AI row: Claude, Gemini, and ChatGPT are pinned by default. Use the "+" button to add any local LLM UI (llama.cpp / Ollama / KoboldAI / text-gen-webui, or any custom http://localhost:PORT) — zero external network calls; everything runs locally on your machine.

    Folders: Default folders include Google, Customize, Movies & Series, Private Chat, Music, and Other — all are fully editable (rename, delete, or add links/apps as needed).

    Weather + live clock (bottom-right): Search for any city worldwide or use the "current location" button. Network requests are made only when you explicitly set your location (powered by Open-Meteo — free, no API key, no tracking). The clock automatically syncs to the timezone of the selected location.

    Settings (gear icon, top-right):

    Appearance: Light/dark/auto theme, dual accent colors (for the Edge-style gradient), customizable backgrounds (upload custom images or pick from Aurora/Sonoma-style gradient presets), wallpaper blur, panel glass opacity, panel vibrancy blur intensity, spring animations, macOS toggles (traffic lights, dock magnify, squircle icons), and the Theme / Shortcut-style pickers.

    Layout: Panel placement (center/top/bottom/left/right), account name, clock format, and panel width/height/scale/corner roundness.

    Apps & Folders: Manage all folders and app links.

    AI: Configure local LLM presets.

    Privacy: Select search engine, export/import configuration settings as JSON, or perform a full system reset.

    Advanced CSS: Apply custom CSS rules directly for full theming control.

# Signing in with a Google Account (Optional)

Navigate to "APIs & Services" → "Credentials" → "Create OAuth client ID" → select Chrome App / Web application as the application type.

    After loading the extension, check your extension ID in about:debugging or about:addons. Add https://<extension-id>.extensions.allizom.org/ as an Authorized Redirect URI (the browser will display this URL in the console or error log if a mismatch occurs).

    Copy your Client ID, paste it into Settings → Profile, and click "Connect Google Account".

Because this connects directly to your personal Google Cloud project without involving any third-party or developer servers, completing these manual setup steps is required.

# Privacy

The extension requests only storage permissions (for saving settings locally) and geolocation permissions (triggered strictly when you press the "current location" button). It contains no analytics, telemetry, or tracking scripts. The complete codebase consists solely of four readable files:
manifest.json, newtab.html, css/style.css, and js/script.js.

# How to Install in LibreWolf / Firefox-based browsers

Option A — Temporary Load (Easiest for testing)

    Open about:debugging#/runtime/this-firefox in LibreWolf.

    Click "Load Temporary Add-on…".

    Select the manifest.json file inside the project directory.

    Open a new tab — your new tab page will update instantly.
    ⚠️ Note: This temporary installation will revert whenever the browser restarts, requiring you to reload the file.

Option B — Permanent Installation (Disabling signing requirements)

    Open about:config in LibreWolf.

    Search for xpinstall.signatures.required and set it to false (LibreWolf officially supports this toggle due to its privacy-focused design).

    Package the project folder into an .xpi file (a standard ZIP archive renamed to .xpi). Then navigate to about:addons → click the gear icon → select "Install Add-on From File".

    Right after installing, Firefox/LibreWolf will ask whether to let the extension control your home page — accept if you want the same launcher on your Home button too, not just on new tabs.

# How to Install in Chrome / Edge / other Chromium browsers

    Open chrome://extensions (or edge://extensions).

    Enable "Developer mode" (top-right toggle).

    Click "Load unpacked" and select the project folder.

    Open a new tab — done. (The homepage_override key is Firefox-only; on Chromium browsers set this page as your home page manually via the browser's own Settings → On startup / Appearance → Show Home button.)

# Customization & Setting Icons

    Right-click any app tile to edit or delete it.

    Click the "+" or "Manage" buttons within a section to add new applications.

    Default app icons use letters or emojis to prevent remote image fetching, maintaining fast performance and high privacy. You can also upload custom local image icons for any app without making requests to third-party servers.

    Switch between the Classic and Sifiomini themes, and between the six shortcut icon styles, from Settings → Appearance — both apply instantly with no reload.

    Turn "macOS traffic-light buttons" and "Dock hover magnify" on or off from Settings → Appearance if you want a flatter, more classic-Fluent look instead.

# Open Source License

Built without build steps, bundlers, or external dependencies — structured purely with standard HTML, CSS, and JavaScript. Free to copy, modify, and redistribute under the MIT License (refer to the LICENSE file for details).

Credits

    Design & Project Lead — UniCone-dev

    Coding Assistance — Claude (Anthropic)
