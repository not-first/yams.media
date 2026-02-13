# The YAMS Command Line: Your Media Server's Best Friend 🛠️

YAMS comes with a super handy command-line interface (CLI) that makes managing your media server a breeze! Think of it as your media server's remote control - but cooler. 😎

## Getting Started

To see what your YAMS CLI can do, just type:
```bash
yams --help
```

You'll get a nice overview of all available commands:

```bash
yams - Yet Another Media Server

Usage: yams [command] [options]

Commands:
--help                     displays this help message
restart                    restarts yams services (can specify service names)
stop                      stops all yams services (can specify service names)
start                     starts yams services (can specify service names)
destroy                   destroy yams services so you can start from scratch (can specify service names)
check-vpn                 checks if the VPN is working as expected
backup                    backs up yams to the destination location
```

Let's break down each command and see what magic they can do! ✨

## The Command Arsenal 🚀

### `yams start`
Fires up your YAMS services. It's like pressing the "ON" button for your media server! You can start all services or specify individual ones. The CLI will even show you a nice progress bar and let you know when everything's up and running (when starting all services).

**Examples:**
```bash
yams start             # Starts all YAMS services
yams start jellyfin    # Starts only the 'jellyfin' service
```

### `yams stop`
Gracefully stops your YAMS services. Think of it as tucking your media server in for a good night's rest. 😴 You can stop all services or specify individual ones. All downloads will be paused, and all services will shut down properly.

**Examples:**
```bash
yams stop             # Stops all YAMS services
yams stop prowlarr    # Stops only the 'prowlarr' service
```

### `yams restart`
Having a hiccup with one of your services? This command is like giving your media server a quick refresh! You can restart all services or specify individual ones.

**Examples:**
```bash
yams restart             # Restarts all YAMS services
yams restart sonarr      # Restarts only the 'sonarr' service
```

### `yams backup [destination]`
Your safety net! 🎯 Backs up your entire YAMS configuration to keep your setup safe. Just tell it where to save the backup:

```bash
yams backup ~/my-backups
```

This will:
1. Stop all services (temporarily)
2. Create a timestamped backup file
3. Start everything back up
4. Tell you exactly where your backup is saved

### `yams check-vpn`
Your privacy guardian! 🛡️ This command makes sure your VPN is doing its job by:
1. Checking your real IP address
2. Checking qBittorrent's IP address
3. Comparing them to make sure they're different
4. Showing you which countries both IPs are from

If something's wrong, it'll let you know right away!

### `yams destroy`
The nuclear option! ☢️ This command completely removes YAMS services so you can start fresh. You can destroy all services, or specific ones. But don't worry - it'll ask for confirmation first! We don't want any accidents. 😅

**Examples:**
```bash
yams destroy             # Destroys all YAMS services, containers, volumes, and the custom network
yams destroy radarr      # Destroys only the 'radarr' service (its container and volume)
```

## Pro Tips 💡

1. **Service Status**: After starting or restarting, YAMS will show you the status of each service, so you know everything's working properly.

2. **Backup Regularly**: Get into the habit of running `yams backup` before making any big changes. Future you will thank present you!

3. **Check That VPN**: Run `yams check-vpn` periodically to ensure your privacy is protected.

## Troubleshooting 🔧

Getting a `docker` permission error when trying to use the CLI? Don't panic! Head over to our [Common Issues](../faqs/common-errors.md) page for the fix.

Remember: YAMS's CLI is here to make your life easier! If you're ever unsure about a command, just add `--help` at the end or check back here for a refresher. Happy streaming! 🎬
