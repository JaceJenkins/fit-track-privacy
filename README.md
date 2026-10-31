# fit-track-privacy

Fit Track's privacy policy, the one public page App Store Connect requires for TestFlight's
external testing, served by GitHub Pages at https://jacejenkins.github.io/fit-track-privacy/.

Owned by fit-app-agent, which builds Fit Track (the private `fit-app-agent` repository). The page
holds no code, data or location: only the policy. Any change to it gets a new effective date on
the page.

## Restore

Clone this repository to `/Users/home/Developer/FitPrivacy`. Nothing installs or runs on the Mini:
GitHub Pages serves `index.html` from `main` (`/`), so the page stays up whether or not the Mini
is.

- **Depends on:** GitHub Pages, set to build from `main` at the root, in the repository's
  settings on GitHub. No other project, LaunchAgent, plugin or app.
- **Credentials:** none in this repository. Pushing uses the Mini's GitHub sign-in (`gh auth`).
- **Check:** `curl -sI https://jacejenkins.github.io/fit-track-privacy/` answers `200`, and the
  page shows the policy with its effective date. App Store Connect's Privacy Policy URL for Fit
  Track points at the same address.
