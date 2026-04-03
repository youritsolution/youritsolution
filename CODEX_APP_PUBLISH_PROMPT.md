# Codex Prompt For New App Publishing

Use this prompt for every new app I want to publish through `youritsolution.dk`.

---

You are helping me publish a new app under `Your IT Solution`.

For this app, follow the same website-and-community pattern we used for `VirtualMac Studio`.

## Goal

Take a new app from “not present on the website” to:

1. added properly to the `youritsolution.dk` website under `Apps`
2. given its own app page
3. given its own support path and support-page links
4. given its own public GitHub feedback hub
5. given its own GitHub Discussions page
6. linked so users can go from the app page and support page to the app’s Discussions page

## Important Website Structure Rules

- The website is a multi-app site.
- Do **not** place the app as a permanent top-level navigation item beside `Apps`.
- Keep the main site navigation in the scalable structure:
  - `Home`
  - `Apps`
  - `Support`
  - `Privacy`
- The app must live under the `Apps` umbrella, not beside it.

## For Each New App, Do This Procedure

### 1. Inspect Existing Website Structure First

Read the current website files in:

- `/Users/samuelyawbaiden/Documents/GitHub/youritsolution`

Especially inspect:

- `index.html`
- `apps.html`
- `styles.css`
- the current app pages already published
- the current support and privacy pages

Preserve the existing website design language unless a change is clearly needed.

### 2. Add The App To The Website

Create or update the website so the new app has:

- an app card under `Apps`
- a dedicated app page
- app-specific support information
- download links if they already exist
- discussion/feedback links

Use the `VirtualMac Studio` site flow as the reference pattern, but adapt it to the new app instead of copying blindly.

At minimum:

- add the app to `apps.html`
- add or update the app page
- add or update the app support page if the app needs its own support page
- ensure the app can be discovered naturally from the homepage and apps page

### 3. Create Or Prepare The Public GitHub Hub

The source code may remain local/private.

For the public side, create or prepare a **public no-source GitHub repo** for the app that acts as:

- public release hub
- issues hub
- discussions hub

Use the same model we used for `VirtualMac Studio`:

- no source code in the public repo unless I explicitly ask for it
- public repo should contain release/support/community-facing files only

If a public app repo does not yet exist:

- create the starter files locally
- if you can publish directly, do so
- if direct publishing is blocked, prepare everything locally and tell me the exact final click(s) I must do

### 4. Make Discussions The Main Feedback Destination

For every app:

- `Discussions` should be the primary general feedback location
- `Issues` should be for bugs and feature requests

From the app page and support page:

- link users to the app’s GitHub `Discussions`
- also link to `Issues`
- link to `Releases` if relevant

The wording should clearly say:

- `Discussions` = feedback, ideas, questions, help, general conversation
- `Issues` = bugs and feature requests

### 5. Update The Support Flow

The app’s support presence must match the current ecosystem:

- website support path
- GitHub Discussions for general feedback
- GitHub Issues for structured bug reports

Where appropriate:

- make the support page point to Discussions first
- keep support email as a fallback, not the main feedback route

### 6. Keep The Site Scalable

Every new app should make the site more reusable, not more custom and one-off.

Prefer patterns that scale to many apps:

- reusable app card structure
- reusable support/discussion wording
- reusable public GitHub repo structure
- reusable release/download layout

If you notice website structure that is too app-specific, improve it while adding the new app.

### 7. Work Autonomously

Do not stop after analysis if you can safely implement.

Reasonable assumptions are allowed when they do not risk data loss or major brand mistakes.

If a step depends on a GitHub feature or website deployment that cannot be completed automatically:

- do as much as possible yourself
- then tell me the exact remaining action in one short concrete step

### 8. Final Output Format

At the end, report back with:

- what website files were created or updated
- what GitHub repo or public hub was created or updated
- whether Discussions are live
- whether the app page links to Discussions
- whether I need to push a repo in GitHub Desktop
- any remaining blocker

## App-Specific Input You Should Expect From Me

When I use this prompt again, I may provide some or all of:

- app name
- app description
- app download artifact
- whether source stays private
- whether a public GitHub repo already exists
- whether support/privacy pages already exist

If some of that is missing, inspect local context first and proceed with reasonable assumptions.

## Current Environment Assumptions

- website repo:
  `/Users/samuelyawbaiden/Documents/GitHub/youritsolution`
- public app repo pattern:
  `/Users/samuelyawbaiden/Documents/GitHub/<AppName>`
- source code may remain local only
- website navigation should stay:
  `Home / Apps / Support / Privacy`

---

When I reuse this prompt, I will append the new app’s name and any app-specific details below it.
