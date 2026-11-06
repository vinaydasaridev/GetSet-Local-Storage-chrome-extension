# Chrome Web Store listing text

Source of truth for the text pasted into the Developer Dashboard (Store listing tab). The name and
summary come from `manifest.json`; only the description is edited in the dashboard. Do not rename the
extension: its name and ID stay as they are.

## Name (from manifest.json)

GetSet Local Storage, Session Storage & Cookies

## Summary (from manifest.json, max 132 characters)

Copy local storage, session storage and cookies from one site to another, e.g. from staging to
localhost. Also clear them.

## Description

GetSet copies a site's local storage, session storage and cookies, then sets them on another site in one
click. Built for developers who need localhost to look exactly like staging or production: the same
feature flags, cached settings, cart and app state, and the same logged-in session, without recreating
it by hand or editing values in DevTools.

How to use it:
1. Open the source site (for example your staging app) and click Get All.
2. Open the target site (for example http://localhost:3000) and click Set All.
3. Reload the target page.

Common uses:
- Reproduce a staging or production bug on localhost with the same user and data.
- Reuse a staging session when your local frontend talks to the staging API.
- Move feature flags, A/B test buckets or onboarding state between environments.
- Reset a site to a clean state with Clear All.

Cookies:
- Chrome asks once per site, the first time you use cookies there. Nothing is asked at install time.
- Copies every cookie the site uses, including HttpOnly cookies, path cookies and parent-domain cookies.
- Keeps secure cookies secure, works on localhost on any port, and keeps each cookie's expiry.
- Incognito stays separate, and Clear only removes the current site's cookies.

Private by design:
- Everything stays in your browser. Nothing is sent to any server, and there is no tracking.
- Copied cookies are kept in memory only and disappear when the browser closes.

Free and open source (MIT):
https://github.com/vinaydasaridev/GetSet-Local-Storage-chrome-extension

Guide and FAQ: https://vinaydasari.com/getset

GetSet is by Vinay Dasari: https://vinaydasari.com
