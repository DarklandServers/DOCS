# SEOW RP Remastered

SEOW RP (Super Epic OMG WTF) is an engaging Garry's Mod roleplay gamemode that immerses players in a dynamic urban landscape where they can assume the roles of cops, thugs, civilians, and even the mayor. The game's central objective revolves around strategic property acquisition, base construction, and the cultivation of a drug empire for profitable sale. Players must adeptly navigate the fine balance between expanding their illegal operations and guarding their assets against rival factions and law enforcement, offering an adrenaline-pumping experience of resource management, competition, and strategic maneuvering within a bustling virtual city.

For detailed information about the features, mechanics, and usage instructions, please refer to the [Documentation](/Docs/README.md).

|          **Game Features**           | **Not Started** | **In-Progress** | **On-Hold** | **Complete** |
| :----------------------------------: | :-------------: | :-------------: | :---------: | :----------: |
| [Core Features](/Docs/pages/CORE.md) |                 |       ✔️        |             |              |
|  [Classes](/Docs/pages/CLASSES.md)   |       ❌        |                 |             |              |
|  [City Living](/Docs/pages/CITY.md)  |       ❌        |                 |             |              |
|   [Thug Life](/Docs/pages/THUG.md)   |       ❌        |                 |             |              |
|   [Realty](/Docs/pages/REALTY.md)    |       ❌        |                 |             |              |
| [Vehicles](/Docs/pages/VEHICLES.md)  |       ❌        |                 |             |              |

## General repo structure

This repository is organized to facilitate collaboration and development on the SEOW RP Remastered gamemode. The main branches are

- **main**: This branch contains the current stable build of the gamemode. It is the version that is considered reliable and suitable for public use.
- **development**: Use this branch for testing and working on major changes. It's the sandbox for implementing and experimenting with new features, mechanics, or improvements.
- **release**: The release branch holds the version of the gamemode that is currently live and playable. It serves as an intermediary step between development and the stable main branch.

## Code Structure for SEOW 2.0

The gamemode is split into modules, each related to a specific portion of the gamemode. File prefixes (sv, cl, sh) determine which state the file will be loaded on. This is done automatically. This includes things such as the hud, money management, chatbox, etc.

The gamemode config is split into four files (found in gamemode/config/)

- **config.lua**: contains information such as general settings, etc
- **classes.lua**: contains information for each playable class
- **achievements**.lua: contains information for each achievement
- **upgrades.lua**: contains information related to global upgrades

content: The content directory contains all materials and sounds for the gamemode. Anything placed in here is auto-added to the client's download - make sure to upload it to the fastdl, too! entities: The entities directory contains things such as the drugs, vehicles, weapons, and much more. Anything the player physically interacts with can be found here.

## Make Life Easy

**Sync Gamemode For Testing**

```
git sync
```

**Push to Repo and Sync the Gamemode**

```
git gamemode "Your Commit Message"
```

[**`Learn More`**](/Docs/README.md)

## Contributing

Contributions to SEOW RP Remastered are welcome! To ensure the project's growth and maintainability, please follow these guidelines:

1. Fork the repository.
2. Create a new branch from the **`'main'`** branch for your bug fix or minor improvement.
3. If you're working on a brand new feature or making a major change, then create a new branch from the **`'development'`** branch.
4. Make your changes and commit them with descriptive messages.
5. Keep your code organized in the proper file and folder structure. This improves readability and maintainability for everyone.
6. Comment your code thoughtfully. Well-documented code helps other contributors understand your intentions and aids in troubleshooting.
7. Push your branch to your fork.
8. Open a pull request to the appropriate base branch (**`'main'`** or **`'development'`**) in this repository.
   <br>
   <br>
   <br>
   > **_Remember to adhere to the project's coding standards and practices._**
   >
   > **_Your contribution will be reviewed and merged if it aligns with the project's goals._**
