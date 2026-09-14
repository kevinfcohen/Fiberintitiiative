# Fiber Field Lab

A mobile-oriented learning PWA and a complete system/training design. This is a synthetic training prototype, not an AT&T-approved work tool.

## Included

- `dist/index.html`: learning app with three skill paths, nine short lessons and six OTDR scenarios.
- `dist/blueprint.html`: full collection, predictive-validation and training-system design.
- `dist/manifest.webmanifest`, `sw.js`, icons: install metadata and offline learning cache.
- `dist/app.js`, `style.css`: dependency-free application source.

## Open or host

Open `dist/index.html` for a local review of the learning interface. Service workers and phone installation need an HTTPS origin (or localhost for development); opening a file is insufficient for these features. Publish the contents of `dist` together at an approved HTTPS location. Preserve relative paths and serve JavaScript and the web manifest with appropriate content types.

On a phone, open the hosted URL, complete any required sign-in, and allow the learning assets to finish caching. Use Safari’s Share → Add to Home Screen on iPhone, or Chrome’s Install app/Add to Home screen on Android where supported. Installation may be restricted by device policy.

The app stores practice progress only in the current browser. Field reference → Clear my practice progress removes those results. Clear site data through the browser to remove cached learning files. There is no production data collection, user account synchronization or employer qualification record.

## Status and verification

Built: all learning views, synthetic interactions, blueprint, install guidance, device-local progress and offline asset code.

Passed: JavaScript syntax; nine lesson definitions and answer keys; six trace scenario outputs; single/dual trace output; pulse and temporal changes; PNG dimensions; manifest and offline asset existence; local HTML links.

Not verified: rendered browser layouts, full UI click-through, phone installation, offline relaunch or managed-device compatibility. Browser execution was blocked in the authoring environment. A GitHub Pages workflow is included. See GITHUB-PAGES.md for activation and deployment details; a live URL must be verified after deployment.

Before organizational use, obtain authorized AT&T procedures, review lesson accuracy and applicability, verify approved hosting/device storage, and test real iPhone/Android installation and airplane-mode relaunch. The source includes no AT&T acceptance thresholds. Training practice does not authorize work.

## Content updates

The service worker cache name is `fiber-lab-v1`. Increment the version when publishing changes to cached content. Only static synthetic assets are cached. Production work instructions need additional approved expiry, revocation and device controls; offline caches are not automatically revoked when hosted access changes.

## Production boundary

Instrument integrations, raw trace ingestion, incident labeling, predictive models, SME case management and training-system integration are specified in the blueprint. They are not implemented by this static learning prototype.


