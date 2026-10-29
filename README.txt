TRIX SIM - app package

1. Put this whole folder on any HTTPS host (Netlify Drop, Cloudflare Pages, GitHub Pages). Opening index.html from disk will not install.
2. Open the URL on your phone. Android Chrome: menu > Install app. iPhone Safari: Share > Add to Home Screen.
   It then launches fullscreen with its own icon and works offline after the first load.
3. Real Android APK: go to pwabuilder.com, paste your hosted URL, choose Android. (Or use Capacitor: npm i @capacitor/core @capacitor/cli @capacitor/android, npx cap init, copy these files into www/, npx cap add android, npx cap open android.)
Note: the three.js and physics libraries load from a CDN on first launch, then are cached by the service worker.
