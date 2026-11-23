# Little Reel: App Store website handoff

The website pages are prepared locally. They become public only after these changes are published to the existing GitHub Pages site. Do not enter the new URLs in App Store Connect until the pages load publicly without signing in.

## URLs after publication

| App Store Connect field | URL |
| --- | --- |
| Marketing URL | https://felderkwek.github.io/macsweeper-site/little-reel/ |
| Support URL | https://felderkwek.github.io/macsweeper-site/little-reel/support.html |
| Privacy Policy URL | https://felderkwek.github.io/macsweeper-site/little-reel/privacy.html |

The app hub will be at https://felderkwek.github.io/macsweeper-site/ . Existing Mac Sweeper support and privacy links remain at `/support.html` and `/privacy.html`.

## Price and availability

The pages describe a planned one-time paid download, without advertising. The price is intentionally not specified. Set the actual price and availability in App Store Connect when ready. Add the final `apps.apple.com` product link to the site after it exists.

## Privacy policy draft and release build

The draft is based on the media import, local project storage, preview, MP4 export, and sharing implementation available in this conversation, plus the owner’s stated ad-free, one-time-purchase model. It distinguishes the app’s local project storage from Apple Photos/iCloud downloads, device backups, email support, and GitHub Pages hosting.

The complete release build and all dependencies were not available for a privacy audit. In particular, `MontageAI.suggest` is referenced by the supplied editor, but its implementation was not available. The owner believes there is no external AI or cloud sync. Verify those facts in the submitted build, along with any analytics or crash-reporting SDKs, before treating the policy as final. The draft does not claim that every part of the app has been audited or that Apple will approve it.

App Store privacy answers must describe the actual release build and third-party dependencies. Do not automatically choose “Data Not Collected” from the absence of ads alone. Update the policy if any data is sent to a service. Review the support-contact retention wording against your actual email-handling practices.

## Website and app submission

Apple requires a public privacy-policy URL and a support page with actual contact information. A website provides those URLs; it does not upload the iPhone app. Upload the signed app build from Xcode to App Store Connect, complete the app’s listing, privacy answers, pricing, and review information, and submit that build for review.

Apple references:

- [Platform version information: Support URL and Marketing URL](https://developer.apple.com/help/app-store-connect/reference/app-information/platform-version-information)
- [App information: Privacy Policy URL](https://developer.apple.com/help/app-store-connect/reference/app-information/app-and-compliance-information)
- [App privacy details](https://developer.apple.com/app-store/app-privacy-details/)
- [Uploading builds](https://developer.apple.com/help/app-store-connect/manage-builds/upload-builds/)

The site has no sign-in wall, remote font dependency, contact form, embedded analytics, or payment form. Support uses the existing public email address, `felderkwek@gmail.com`.
