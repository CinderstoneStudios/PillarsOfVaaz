# Pillars of Vaaz
A repository of public data that defines how live content from the Prominence modpacks works.

## The Purpose
The goal of this repository is to define:
1. List of developer UUIDs for dev-only features like the dev badges, used to identify actual modpack devs in servers.
2. Dynamic configs, which are explained in depth below.

## Dynamic Configs
This is the foundation of our live content. We are going to use this to ship weekly quests, entire seasonal questlines, mythic rotations, or featured listings in real time, everything synced across all versions.

### Security Concerns
The system has been built to be as safe as possible, since its only purpose is to ship configuration files for live content, and guarded behind this official repo with a hardcoded call from all clients.

We've implemented these simple but efficent safety measures, just in case:
- Files will only be downloaded by clients if they are of the following formats:
  - .json  .json5  .jsonc  .conf  .toml  .yaml  .properties  .configuration
  - .snbt (Only works for ftbquests folders)
- Files are always downloaded inside the game's config folder, with no way to escape outside it.

We've also included a way to opt out of this system, by going to config/prominent/live_content.json5 and disabling live content altogether.

# License
The contents of this repository are All Rights Reserved, Copyright Cinderstone Studios LLC, unless explicitly stated.
