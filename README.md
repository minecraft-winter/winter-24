# Winter 2024 Modpack

# Game Setup

- Download the 'jars' zip from the [latest release page](https://github.com/minecraft-winter/winter-24/releases/latest)
- Extract it into your minecraft mods folder. On windows, that's `%AppData%/.minecraft/mods`.

You can also use the 'client' zip if you're using a CurseForge-compatible launcher like [Prism Launcher](https://prismlauncher.org/), [PolyMC](https://polymc.org/), or any of the many others.

# Contributing

## Setup

Install [packwiz](https://packwiz.infra.link/installation/) and [git](https://git-scm.com/). The latest `packwiz` build can be found attached [here](https://github.com/packwiz/packwiz/actions/workflows/go.yml). Click the latest successful run and scroll down to 'Artifacts' to find the appropriate build for your system. Extract the build and add it to your path as noted in the `packwiz` docs.

## Using Packwiz

The [Packwiz docs](https://packwiz.infra.link/tutorials/creating/getting-started/) have more details. Three of the most common commands are documented here.

### Add Mods

`packwiz curseforge add <URL>`

## Update Mods

`packwiz update --all`

## Testing Locally

`packwiz modrinth export --output jars.zip`

# Releasing a New Modpack Version

1. Update version in `pack.toml`
2. Commit this change
3. Send a PR
4. Once the change is merged, I'll:
5. Tag the new version in the format `v*.*.*`
6. Push the tag

This will kick off a release automation that will create a new Github release and attach a set of modpack zips to it.
