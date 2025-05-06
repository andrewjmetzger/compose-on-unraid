---
title: "Installing compose"
weight: 1
---

## Introduction

A new Unraid plugin, [Docker Compose Manager] brings native Docker Compose functionality directly to your Unraid server. With this plugin installed, you can deploy and manage container stacks using both the command line as well as a new, integrated web UI—much like the streamlined experience that Docker Templates provide. This page will walk you through installing the plugin (referenced from the official [Docker Compose Manager forum thread][Docker Compose Manager]) and setting it up step by step.

## Prerequisites

Before you begin, make sure you have:
  
1. A running and up-to-date Unraid server, version 6.10.0 or later.
2. Administrative access to the Unraid web UI.
3. The Community Applications plugin installed (if you don’t have it yet, follow the instructions below).

## Step 1: Install Community Applications (if not installed)

1. **Log in** to your Unraid web UI.
2. Navigate to the **Apps** tab.
3. If Community Applications is not already installed, the page offers an Install button. No need to hunt for the plugin link!

## Step 2: Install Docker Compose Manager

1. Once Community Applications is available, click on the **Apps** tab in the Unraid web UI.
2. In the search bar, type **Docker Compose Manager**.
3. Locate the plugin in the search results and click the **Install** button.
4. Follow any on-screen instructions to complete the installation. During installation, the plugin will deploy Docker Compose along with the compose switch, ensuring you can use both `docker compose` and `docker-compose` commands.

## Step 3: Verify the Installation

1. Open the **Docker** tab in your Unraid interface.
2. Look for a new control section dedicated to Docker Compose Manager. This section should let you create, edit, and execute Docker Compose YAML files.
3. For additional confirmation, open a terminal window and run: `docker compose version`. The command should return the Docker Compose version information.

[Docker Compose Manager]: https://forums.unraid.net/topic/114415-plugin-docker-compose-manager