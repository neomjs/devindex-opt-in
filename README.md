# DevIndex Opt-In

This repository serves a single purpose: providing an automated way for developers to opt in or nominate others for **[DevIndex](https://neomjs.com/dist/production/apps/devindex/index.html)** — the index of the 50,000 most active developers on GitHub, ranked by lifetime contributions.

DevIndex is radically inclusive by design. The Spider that discovers profiles is a heuristic, not a database dump, so it **will** have gaps — quite possibly including people with hundreds of thousands of contributions. This repository is how those gaps get closed.

## How to Opt-In

There are two ways to be added.

### Option 1: The "Quick Star" Method (for yourself)

To add your own profile, **Star this repository** at the top right of this page.

**What happens next?**
1. Our automated discovery pipeline runs hourly.
2. It detects your star, automatically verifying your GitHub identity.
3. Your GitHub username is added to our tracking queue.
4. The updater evaluates your metrics. If your total contributions meet the current entry threshold, your profile is indexed and displayed. If not, you are removed from the queue — you are welcome to submit a new request once your contributions have grown.

**Note:** You can safely un-star this repository after a few hours. The opt-in is permanent unless you later decide to [opt out](https://github.com/neomjs/devindex-opt-out).

### Option 2: Issue Templates (for yourself, or to nominate others)

If you prefer a documented request, or want to nominate developers you think should be featured:

1. Go to the **Issues** tab of this repository.
2. Click **New Issue**.
3. Choose either **DevIndex Opt-In (Myself)** or **DevIndex Opt-In (Nominate Others)**.
4. Fill out the form and submit.

The pipeline processes these hourly, verifies the usernames, and adds them to the tracking queue.

## The entry threshold

DevIndex holds the top 50,000 developers, and the bar rises as it fills — it is whatever 50,000th place currently costs, not a fixed rule. Meeting it is the only gate; there is no editorial judgement involved.

## Where things live

| Repository | Purpose |
|---|---|
| [neomjs/devindex](https://github.com/neomjs/devindex) | The application and the Data Factory that processes these requests |
| [neomjs/devindex-opt-out](https://github.com/neomjs/devindex-opt-out) | Removal requests |

Full detail on how opt-in is processed: [Opt-In & Nominations](https://github.com/neomjs/devindex/blob/main/learn/OptIn.md). For what gets indexed and why, see [The Ethical Manifesto](https://github.com/neomjs/devindex/blob/main/learn/EthicalManifesto.md).

Bugs and feature requests belong on the [DevIndex tracker](https://github.com/neomjs/devindex/issues) — this repository is for opt-in requests only.
