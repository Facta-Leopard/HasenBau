# HasenBau · public website

Official bilingual Korean/English support and privacy website for the HasenBau iPad app. Each section shows both languages together. No build step, JavaScript, remote fonts, analytics, advertising scripts or form backend.

## App Store Connect URLs

| Field | URL |
| --- | --- |
| Marketing URL / Developer Website | https://facta-leopard.github.io/HasenBau/ |
| Support URL | https://facta-leopard.github.io/HasenBau/support.html |
| Privacy Policy URL | https://facta-leopard.github.io/HasenBau/privacy.html |
| Privacy Choices URL (optional) | https://facta-leopard.github.io/HasenBau/privacy.html#contact |

Use the same URLs for Korean and English localizations. Public support/privacy contact: `shteosis@gmail.com`, reused from the owner's existing developer support website. Do not send full learner backups through public GitHub issues.

## Hosting

GitHub Pages publishes `main` at the repository root. `.nojekyll` serves the static files unchanged. Preview with `python3 -m http.server 8768 --bind 127.0.0.1` from this folder. Application source and learner data are not part of this repository.

## AdMob preparation

The canonical seller file is **https://facta-leopard.github.io/app-ads.txt**, maintained in `Facta-Leopard/Facta-Leopard.github.io`. Its existing, publicly verified entry is:

```text
google.com, pub-7572108671787552, DIRECT, f08c47fec0942fa0
```

The project-level `app-ads.txt` is a matching convenience copy. It does not replace the domain-root file. Google derives the hostname from the App Store **Marketing URL**, so keep the URL above in the store listing. No changes to the shared root site were needed. A reachable file is not evidence of AdMob account verification; connect the released store listing and check its app-ads.txt status in AdMob.

Before serving ads, integrate the applicable Google SDK/consent flow, review the actual privacy report and App Store data disclosures, and update the current-status text in `privacy.html` and `support.html`. Do not describe test-mode SDK requests as “no data collection.” This website itself serves no ads.

Official references checked October 7, 2026:
- [Google: set up app-ads.txt](https://support.google.com/admob/answer/9363762?hl=en)
- [Google: iOS data disclosure](https://developers.google.com/admob/ios/privacy/data-disclosure)
- [Google: UMP consent](https://developers.google.com/admob/ios/privacy)
- [Apple: App privacy fields](https://developer.apple.com/help/app-store-connect/reference/app-information/app-privacy/)

## Assets and rights

`assets/icon.png` is the owner-supplied HasenBau icon, copied from the app's BrandIcon asset. `assets/artwork.png` is its original 1254px artwork, copied from SplashArtwork for the larger hero image. `assets/hanji.png` is the paper texture generated for HasenBau and copied from its PaperHanji asset. The app's provenance record is `Docs/PAPER_ART.md` in the local app project. These files are copied unchanged. No third-party font, CSS framework or JavaScript package is redistributed. This repository does not grant a general license to reuse the app artwork or branding.
