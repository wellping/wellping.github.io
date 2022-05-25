# [wellping.github.io](https://wellping.github.io/)

This repo contains the user-/researcher-facing website for Well Ping, as well as some universal links-related setup files for the wellping.github.io domain.

## Universal Links (for the `app/` folder)

If the user has installed the app, they will be able to launch the app by visiting any page under https://wellping.github.io/app/ (the `app/` folder). This is very useful for pre-filling the login information, as the user simply has to click a link in the email they received to automatically have the app opened and their user login code entered.

This is set up on the web-side by the [`.well-known` folder](#well-known-folder) and on the client-side by `ios.associatedDomains` and `android.intentFilters` keys in https://github.com/wellping/wellping/blob/master/app.json.

See https://docs.expo.io/workflow/linking/#universaldeep-links-without-a-custom-scheme for more information.

### `.well-known` folder

The `.well-known` folder stores files necessary for iOS (the [apple-app-site-association](./.well-known/apple-app-site-association) file) and Android (the [assetlinks.json](./.well-known/assetlinks.json) file) to recognize `wellping.github.io` as the domain to open the Well Ping app when the user visits any page under the `app` folder https://wellping.github.io/app/.

Learn more: https://github.com/wellping/wellping/issues/20.
