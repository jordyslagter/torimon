---
slug: "/"
sidebar_position: 0
---

# Setting up a development environment

## Prerequisites

- [Go](https://go.dev/)
- [PrismLauncher](https://www.prismlauncher.org/)
- [OpenJDK 21](https://www.adoptium.net/temurin/releases/?os=any&arch=any&version=21)

## Install Packwiz

```bash
go install github.com/packwiz/packwiz@latest
```

## Set up development instance of Minecraft

Open PrismLauncher and add a new instance with the _Fabric_ version listed in
[_pack.toml_](https://github.com/jordyslagter/torimon/blob/main/torimon/pack.toml)
and run the instance once.

Download and add the latest
[Packwiz Development installer](https://www.github.com/packwiz/packwiz-installer-bootstrap/releases)
to the minecraft/ directory of the instance, make sure it is called
_packwiz-installer-bootstrap.jar_. See below for the directory structure.

```
minecraft/
- packwiz-installer-bootstrap.jar
```

Now go into the settings of your instance, enter the _Custom Commands_ tab.
Enable _Custom Commands_ and add the following as the pre-launch command:

```bash
"$INST_JAVA" -jar $INST_MC_DIR/packwiz-installer-bootstrap.jar http://localhost:8080/pack.toml
```

Now your instance is ready to be used for development and testing!

## Launch the modpack in the development instance

Clone the git repository.

```bash
git clone https://github.com/jordyslagter/torimon.git
```

Enter the repository.

```bash
cd torimon/torimon
```

Run packwiz for development.

```bash
packwiz serve
```

Now you can run your development instance and it will sync with your local changes.

Refer to the
[packwiz tutorial](https://packwiz.infra.link/tutorials/creating/getting-started/)
for adding, removing and pinning mods.
