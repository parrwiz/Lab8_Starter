# Lab8-Starter

## Lab Partners
* Parwiz Khan

## GitHub Pages Deployment


---

## Q1: How are graceful degradation and service workers related?

**A1:**  
Graceful degradation is the idea of starting with a fully featured application and ensuring it still functions well when features are removed or limited. Service workers help achieve graceful degradation by allowing web applications to continue functioning even when the network is unavailable. If a user loses connection, the service worker can serve cached assets instead of breaking the app. This ensures a resilient user experience, making the app degrade “gracefully” rather than fail completely.

---

## Q2: Try installing on your other devices (phone, tablet, etc.) What happens?

**A2:**  
When i load on my phone, the title is as written in `index.html` and When I installed it on my phone's homescreen, I noticed that the app name shown under the icon is taken from the `short_name` field in the manifest file — not the full `name`.

If the manifest and service worker are set up correctly, mobile browsers (like Chrome) will offer an install prompt. Once installed, the app appears on the home screen, runs in standalone mode, and can even work offline thanks to the service worker. The experience feels like a native mobile app, supporting touch input, splash screens, and custom icons.
