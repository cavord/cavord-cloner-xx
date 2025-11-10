# cavord-cloner-xx

## What is this?

A small README that explains a tool which clones a Discord server. The tool copies everything from an original server into a "clone" server so you can restore it if the original was nuked or raided.

## Main features

The tool can:

* **Delete everything in the clone server** before copying, so the clone becomes a fresh copy.
* **Copy categories** (with names and order).
* **Copy channels** (text & voice) and **copy channel permissions** so channels keep the same access rules as the original.
* **Copy roles** and **copy role permissions** (position and color are preserved if possible).
* **Copy emojis** from the original server.
* **Copy server name** and **server profile picture (pfp)**.

In short: it tries to make the clone look and behave like the original server.

## Why use it?

If a server is attacked (nuked/raided) or accidentally broken, a prepared clone helps restore structure and settings quickly.

## Requirements (high level)

* A bot or account token with the right permissions on both servers (read/manage channels, manage roles, manage emojis, change server settings).
* The clone server must allow the bot/account to make the changes.

> **Important:** Do not use this tool to copy servers you do not own or do not have permission to copy. Always respect Discord Terms of Service and the server owner's rights.

## Basic usage (example)

1. Provide the **original server ID** and the **clone server ID** to the tool.
2. Optionally enable a `clear_clone` option to delete everything in the clone before copying.
3. Run the clone process. The tool will:

   * Clear clone (if enabled).
   * Create roles, categories, channels in the same order.
   * Copy role permissions and channel permission overwrites.
   * Upload emojis.
   * Update clone name and pfp.

## Permissions the tool needs

* Manage Server (to change name & icon)
* Manage Roles
* Manage Channels
* Manage Emojis
* Read Messages / View Channels
* Manage Permissions

## Safety & ethics

* Use only for backup, recovery, or with explicit permission from the server owner.
* Keep tokens and credentials secret.
* Test on a small sample server first.
* Back up data exported from the original server before mass changes.

## Limitations

* Some features (like some 3rd-party integrations, server boosts, Nitro-exclusive emojis or features) cannot be copied.
* Rate limits: Discord API rate limits may slow the process or require retries.

## Support / Contact

If you want the README adjusted (more technical detail, commands, or example code), tell me what you want and I will update it.
