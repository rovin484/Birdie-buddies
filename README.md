# Birdie Buddies — iPhone prototype v1

This is a mobile-friendly web app prototype for the Birdie Buddies golf concept.

## What works in v1
- Requests the iPhone's GPS location and shows it on a map.
- Lets the golfer tap the map to mark an estimated ball landing location.
- Calculates straight-line distance from the phone to the marked location.
- Opens Apple Maps walking directions to the marked location.
- Opens the iPhone camera in Safari (where supported) and records a short clip.
- Includes an editable 18-hole scorecard, lost-ball counter, and saved shot history.
- Saves scorecard and shot-history data in the browser on the device.

## Important prototype limitation
This version does **not** automatically detect or track a golf ball with AI. The golfer manually marks the estimated landing spot on the map. The camera is included to demonstrate shot recording and to provide a starting point for future computer-vision development. GPS reports the phone's location, not the ball's location. Distance and location estimates are approximate.

## Run it on an iPhone
Camera and GPS permissions generally require a secure HTTPS website. Opening `index.html` directly as a local file may not allow those features.

### Simple hosting route: GitHub Pages
1. Unzip this folder on a computer.
2. Sign in to GitHub and create a new **public** repository named `birdie-buddies`.
3. Upload the five files in this folder to the repository's root: `index.html`, `manifest.json`, `service-worker.js`, `icon-192.png`, and `icon-512.png`.
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**, select branch `main` and folder `/ (root)`, then save.
6. Wait for GitHub Pages to publish the site. The address will look like `https://YOUR-USERNAME.github.io/birdie-buddies/`.
7. Open that HTTPS address in **Safari on your iPhone**.
8. Tap the Share icon → **Add to Home Screen** → Add.
9. Open Birdie Buddies from the new Home Screen icon. Allow location and camera access when prompted.

## How to use it
1. Open the Track tab and tap **Enable GPS**. Allow location access.
2. Enter a course name and choose the current hole.
3. After a shot, tap the map at the estimated landing location.
4. Read the approximate distance from your current phone location to the marked spot.
5. Tap **Navigate to ball** to open Apple Maps.
6. Optionally open the camera and record the shot.
7. Tap **Save shot location** to add the marker to History.
8. Use Scorecard to edit strokes and track lost balls.

## Notes
- Map tiles require an internet connection.
- For the best experience, allow Safari location access and use the app outdoors with a clear GPS signal.
- Do not rely on this student prototype for official scorekeeping or precise golf measurements.
