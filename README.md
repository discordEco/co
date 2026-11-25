# POE2 Collector

An independent, non-commercial community information tool for Path of Exile 2, built on Reddit's Devvit platform. It is not affiliated with Reddit or Grinding Gear Games.

## Current status (v0.5.0)

Private development and testing only. Manual browsing of new and hot posts from the test community and r/PathOfExile2 is implemented. An administrator-only scheduled collector supports 15, 30 or 60 minute intervals, recent-post filtering, duplicate detection and operational statistics. Scheduled operation with the browser closed has not yet been fully verified.

Gemini and Discord connectivity have been tested successfully using fixed synthetic messages only. Actual Reddit content is not sent to either service by the current integration routes.

## Proposed functionality — not yet enabled

Subject to Reddit authorization, applicable policies and any necessary community permissions, the app would translate and summarize selected public discussions in Korean and deliver short summaries with original Reddit links to a dedicated Discord channel. No Reddit data is intended for AI training, fine-tuning, advertising or unrelated content recommendations. Before activation, deletion handling, retention limits, provider data-use terms and access controls must be verified.

## Development

The Devvit project uses TypeScript, React, Hono and Devvit Redis. The scheduler checks every 15 minutes; collection frequency is configurable. Manual results are displayed inside Reddit. Scheduled collection stores recent post IDs and operational statistics rather than post bodies.

App settings: `geminiKey` (secret), `discordWebhook` (secret), `geminiModel` (model identifier). Never commit credentials, webhook URLs, `.env` files or private logs. Rotate exposed credentials. External test requests are limited to ten per service per UTC day.

For the existing Devvit project, use `npm install`, `npm run test:types`, `npm run build`, and `npm run dev` for local development/playtesting. These documentation files alone are not a runnable application.

## Policies and contact

- [Terms of use](TERMS.md)
- [Privacy policy](PRIVACY.md)
- [Project issues](https://github.com/discordEco/co/issues) (do not include secrets or private information)
- [Reddit Developer Platform](https://developers.reddit.com/)

External content processing must remain disabled until authorization and safeguards are confirmed.
