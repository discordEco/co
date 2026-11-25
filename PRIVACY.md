# POE2 Collector — Privacy Policy

Last updated: November 26, 2026

## 1. Scope and operator

This policy describes the current private test version (v0.5.0) of POE2 Collector, an independent non-commercial Devvit app. The project maintainer operates the app; Reddit, Google and Discord independently process information under their respective policies.

## 2. Information processed

Manual collection retrieves public Reddit post IDs, titles, bodies, author names, creation times, scores, comment counts and original links for display inside the app. The app checks the current Reddit username and community to restrict scheduled collection controls and external connectivity tests to the test administrator. It does not intentionally request private messages, email addresses or passwords from readers.

Scheduled collection reads recent public posts and stores collection settings, post IDs with timestamps, counters, scheduling information and up to 20 recent operational log entries in Devvit Redis. The scheduled collector does not intentionally persist post bodies or author names. Manual browsing may hold results and duplicate-tracking information in the browser session; preferences may be stored locally.

## 3. Purpose and retention

Information is used to display community discussions, avoid duplicate collection, administer scheduling and diagnose failures. The scheduled collector prunes IDs older than seven days during collection; this is not a guaranteed seven-day deletion deadline if collection stops. Settings, statistics and recent logs may remain until replaced or manually cleared. External test quota counters expire after approximately 48 hours. Reddit and hosting-provider logs may have separate retention periods outside the app's control.

## 4. External services

Current Gemini tests send a fixed synthetic translation prompt to Google; Discord tests send a fixed synthetic connection message to a configured webhook. No actual Reddit post content is sent through these test routes. Credentials are stored in Devvit secret settings and are not intended for public display. Providers may process request metadata and test messages under their own policies.

Proposed Korean translation, summarization and Discord delivery of real Reddit content remain disabled pending authorization. Before activation, this policy must be updated to describe actual transferred fields, provider retention and data-use terms, deletion propagation and access controls. Reddit data is not intended for AI training or fine-tuning, sale or advertising.

## 5. Security and deletion

The app uses administrator checks for scheduled controls and integration tests, secret settings for credentials and request limits. These measures do not guarantee absolute security. Exposed credentials should be revoked and replaced. Automatic deletion synchronization with external services is not implemented in the current test version. Requests concerning retained data can be reviewed by the maintainer; removal from independent third-party systems cannot be guaranteed by this app.

## 6. Contact and rights

For privacy questions or deletion requests, use the [project issue tracker](https://github.com/discordEco/co/issues) to request a private contact channel without posting personal information. A private contact method and a verified deletion process must be established before public launch. Applicable privacy rights remain unaffected.

## 7. Changes

This policy will be updated before enabling material new data uses or public deployment.
