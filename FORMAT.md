# The format: every app follows it

Free, for everyone, everywhere. No ads, no accounts, no tracking, no app stores, no money.

## Checklist

- [ ] **Static.** HTML, CSS, JavaScript. No server. At most a tiny build script, and the built file is committed so GitHub Pages needs no build.
- [ ] **Installable.** `manifest.webmanifest`, icons (192, 512, maskable 512, apple-touch 180 without transparent corners), `<link rel="manifest">` on every page.
- [ ] **Works offline.** `sw.js` saves what the app needs on the first visit. Test: open once, switch to airplane mode, reload.
- [ ] **No outside requests.** Fonts, images, scripts and libraries live in the repo. No Google Fonts, no CDNs (blocked in China, and they leak visits). Test: DevTools → Network shows only your own address.
- [ ] **No accounts, no personal data on servers.** If the app must recognise someone: a code word plus the phone's local storage.
- [ ] **Languages.** A switch at the top: English and German at least, Chinese where it makes sense. Starts in the phone's language, remembers the choice on the phone.
- [ ] **Accessible.** Text at least 16 px (18 is nicer), good contrast in light and dark mode, tap targets at least 48 px, real buttons and labels for screen readers, visible focus, respects reduced motion.
- [ ] **Phone first.** Check at 390 × 844 before anything else.
- [ ] **Open.** Public GitHub repo, MIT `LICENSE`, hosted on GitHub Pages. Fonts and data keep their own licences (e.g. SIL OFL) next to the files.
- [ ] **Same small shell.** Name, one-sentence description, icon, install help for Android and iPhone, "free, no ads, no account, no tracking", link to the code.
- [ ] **On the hub.** A card on the hub: icon, one line, languages, works offline, open.

## Exceptions

Apps that hold other people's data (players, patients, an organisation's stock) stay private and may use a server. Personal gifts with real names and photos: ask the people first.
