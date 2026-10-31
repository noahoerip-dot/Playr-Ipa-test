# Playr IPA builder

You do not need a Mac or Xcode. GitHub builds the app for you for free.

## Build the IPA
1. Make a free account at github.com and create a new repository (private is fine).
2. Upload everything in this folder to it, including the hidden `.github` folder
   (easiest: on the repository page choose "Add file" > "Upload files" and drag the
   whole unzipped folder in).
3. Open the "Actions" tab. Choose "Build Playr IPA" and press "Run workflow".
4. After about 5 to 10 minutes open the finished run and download `Playr-ipa`.
   Unzip it to get `Playr.ipa`.

## Install it on your iPhone
The IPA is unsigned, so a sideloading tool signs it with your own Apple ID:
- Sideloadly (sideloadly.io, Windows or Mac), or
- AltStore (altstore.io, Windows or Mac).

With a free Apple ID the app works for 7 days, then you install it again.

## Notes
- Your music files and settings stay inside the app on the phone.
- To change the app, replace `www/index.html` and run the workflow again.
- Spotify login does not work inside this app, because Spotify only accepts https
  redirect addresses. Local files, lyrics and everything else work.
