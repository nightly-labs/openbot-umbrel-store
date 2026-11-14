# OpenBot for Umbrel

The [Umbrel](https://umbrel.com) community app store of [OpenBot](https://openbot.run). It has one app,
`openbot-server`: an OpenBot server of your account on your Umbrel. You use it from the OpenBot desktop
app, the OpenBot phone app or `openbot.run/app`.

## Install

1. On your Umbrel, open the **App Store**.
2. Open the **⋯** menu at the top right and select **Community App Stores**.
3. Paste `https://github.com/nightly-labs/openbot-umbrel-store` and select **Add**.
4. Open the **OpenBot** store and install **OpenBot**.
5. Open the app from the home screen and sign in with the email code of your OpenBot account.

Then open OpenBot on your computer, on your phone or at `openbot.run/app`, sign in with the same email
and select the server. The full guide is
[docs/umbrel.md](https://github.com/nightly-labs/openbot/blob/main/docs/umbrel.md).

## Updates

The workflow `.github/workflows/update.yml` looks for a new OpenBot release each six hours. It makes the
app folder with `scripts/umbrel-app.ts` of that release, which pins the image by its digest, and commits
it. Umbrel then offers the update. Do not edit the app folder by hand: the next update replaces it.

OpenBot is source-available under the
[PolyForm Noncommercial License 1.0.0](https://github.com/nightly-labs/openbot/blob/main/LICENSE).
