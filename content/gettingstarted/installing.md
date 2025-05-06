---
title: "Installing compose"
weight: 1
---

## Introduction

A new Unraid plugin, [Docker Compose Manager] brings native Docker Compose functionality directly to your Unraid server. With this plugin installed, you can deploy and manage container stacks using both the command line as well as a new, integrated web UI—much like the streamlined experience that Docker Templates provide. This page will walk you through installing the plugin (referenced from the official [Docker Compose Manager forum thread](https://forums.unraid.net/topic/114415-plugin-docker-compose-manager/) ) and setting it up step by step.

## Prerequisites

Before you begin, make sure you have:
  
1. A running and up-to-date Unraid server, version 6.10.0 or later.
2. Administrative access to the Unraid web UI.
3. The Community Applications plugin installed (if you don’t have it yet, follow the instructions below).

## Step 1: Install Community Applications (if not installed)

1. **Log in** to your Unraid web UI.
2. Navigate to the **Plugins** tab and click on **Install Plugin**.
3. In the URL field, enter: https://raw.githubusercontent.com/Squidly271/community.applications/master/plugins/community.applications.plg
4. Click **Install** and wait until the installation process finishes.  
This plugin is the gateway to installing many popular community plugins easily.

## Step 2: Install Docker Compose Manager

1. Once Community Applications is available, click on the **Apps** tab in the Unraid web UI.
2. In the search bar, type **Docker Compose Manager**.
3. Locate the plugin in the search results and click the **Install** button.
4. Follow any on-screen instructions to complete the installation. During installation, the plugin will deploy Docker Compose along with the compose switch, ensuring you can use both `docker compose` and `docker-compose` commands.

## Step 3: Verify the Installation

1. Open the **Docker** tab in your Unraid interface.
2. Look for a new control section dedicated to Docker Compose Manager. This section should let you create, edit, and execute Docker Compose YAML files.
3. For additional confirmation, open a terminal window and run: `docker compose version`. The command should return the Docker Compose version information.

## Step 4: Configure Docker Compose Manager

1. Click on the new **Compose Manager** control tab within the Docker section.
2. Use the interface to **create new compose files** or edit existing ones directly from your browser.
3. Start your containers by clicking **Compose Up** and stop them with **Compose Down**.
4. If you need to work with environment variables, take advantage of the plugin’s option to specify a custom `.env` file––simply input the path in the settings panel.
5. Adjust any additional configuration options as required by your deployment needs.

## Step 5: Testing Your Configuration

1. To test, create a simple Docker Compose YAML file using the web UI.
2. Execute the command by clicking **Compose Up** and verify that your test container is running as expected.
3. For further details on command syntax and advanced options, consult the official [Docker Compose documentation](https://docs.docker.com/compose/cli-command/).

## Troubleshooting & Next Steps

- **Plugin Visibility:** If the Compose Manager tab isn’t showing in your Docker view, refresh your browser and double-check the Community Applications installation.
- **Command Line Issues:** Make sure you’re using the correct command variants (`docker compose` vs. `docker-compose`).
- **YAML Errors:** Validate your YAML file syntax if you encounter errors during deployment.
