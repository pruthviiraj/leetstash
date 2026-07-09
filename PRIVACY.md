# Privacy Policy for LeetStash

Last updated: July 9, 2026

LeetStash is an unofficial browser extension that helps you push accepted LeetCode solutions to a GitHub repository you choose. The extension has no backend server. Its core features run in your browser and use the external services you configure.

This policy explains what data the extension handles, why it handles that data, where data is sent, and how you can control it.

## Data the extension handles

The extension may store the following data in Chrome extension local storage (`chrome.storage.local`) on your device:

- GitHub personal access token, used only to call the GitHub API on your behalf.
- Optional Groq API key, used only if you add your own key for AI-drafted approach notes.
- Repository settings, including owner, repository, branch, folder, formatting preferences, and auto-push settings.
- LeetCode solution metadata, including problem title, problem slug, difficulty, language, topics, runtime or memory values when LeetCode reports them, and sync dates.
- Your solution code, problem notes, complexity notes, generated README content, pending push queue, and local sync history.

The extension does not use analytics, advertising SDKs, tracking pixels, cookies for tracking, or third-party telemetry.

## Where data is sent

The extension sends data only as needed to provide its stated functionality:

- GitHub (`https://api.github.com`): Your configured repository receives solution files, generated README files, commit metadata, and GitHub API requests authenticated with your GitHub token.
- LeetCode (`https://leetcode.com` and `https://leetcode.cn`): The extension reads problem metadata, accepted submission details, and page content from the LeetCode page you are using. It uses your existing LeetCode browser session and does not post solutions to LeetCode.
- Chrome on-device AI: When available, approach drafting may run locally in Chrome. In that case, the draft is generated on your device.
- Groq (`https://api.groq.com`): If you save a Groq API key and request an AI draft, the problem statement and solution code may be sent to Groq to generate the draft.
- Pollinations (`https://text.pollinations.ai`): If Chrome on-device AI is unavailable, no Groq key is configured, and you request an AI draft or enable auto-draft, the problem statement and solution code may be sent to Pollinations as a keyless fallback.

If you do not want solution code or problem text sent to Groq or Pollinations, do not use the Draft button, disable Auto-draft approach, and leave the Groq API key field empty.

## How data is used

The extension uses the data it handles to:

- Detect the current LeetCode problem and accepted solution.
- Create solution files, problem READMEs, language indexes, and repository indexes.
- Push commits to the GitHub repository you configured.
- Show local sync stats, streaks, recent syncs, pending pushes, and per-problem notes.
- Generate optional approach drafts when you request that feature.
- Export or import your local backup from the options page.

## Data sharing and sale

The extension does not sell, rent, or transfer user data to information resellers, data brokers, advertising networks, or creditworthiness services.

The extension does not use user data for advertising, retargeting, personalized ads, or unrelated product analytics.

Data is shared only with the external services listed above when required for the user-facing features you choose to use.

## Data retention and deletion

Local extension data remains on your device until you delete it.

You can delete or control your data by:

- Clicking Reset setup in the extension popup to remove your saved configuration and token.
- Removing the extension from Chrome, which deletes extension local storage.
- Using the options page to export a backup or import a replacement backup.
- Deleting files or commits from your GitHub repository using GitHub.

GitHub, Groq, Pollinations, and LeetCode may retain data according to their own privacy policies and account settings.

## Security

All external requests use HTTPS. GitHub and Groq API keys are stored in Chrome extension local storage on your device. Because browser local storage is accessible to the extension, use this extension only on a trusted personal machine and avoid sharing exported backups that include tokens.

## Children

This extension is intended for developers and coding learners. It is not directed to children under 13, and the extension does not knowingly collect data from children.

## Changes

This policy may be updated when the extension changes how it handles data. The latest policy should be published at the privacy policy URL listed in the Chrome Web Store Developer Dashboard.

## Contact

For privacy questions, open an issue on the extension's public GitHub repository or contact the developer email listed on the Chrome Web Store listing.
