# Ultramarine-CraftEngine | [中文](README.md)

> A port of the Chinese ancient architecture mod [Ultramarine](https://github.com/LocusAzzurro/Ultramarine) to Paper servers via [CraftEngine](https://github.com/Xiao-MoMi/craft-engine).

## About

[Ultramarine](https://modrinth.com/mod/ultramarine) is a cosmetic mod inspired by ancient Chinese wooden architecture and interior design, adding hundreds of building blocks, decorative elements, furniture and survival materials.

This project converts its content (blocks, items, furniture, recipes, ore generation, loot, localization and resource pack) into CraftEngine configurations, running on **Paper / Spigot / Folia** servers:

- **Server-side only**: Players don't need to install any mod — just the resource pack delivered by the server.
- **Complete content port**: Building blocks, carved elements, furniture, porcelain, ores and crafting recipes are all included.
- **Vanilla-style textures**: All 16×16 textures blend naturally with vanilla blocks.

Current version: `0.0.3`

> [!TIP]
>
> Pictures show only some items

![Ultramarine-Preview](image.png)

> [!WARNING]  
> ### Some blocks may require the client mod!  
> Some blocks use vanilla block states, and the [client mod](https://modrinth.com/mod/craftengine-client-mod) is required to fix visual issues

## Content Overview

| Category | Count | Description |
| --- | --- | --- |
| Building Blocks | 60+ | Cyan bricks, black bricks, brownish red stone bricks, floor tiles, roof tiles and ridges, etc. |
| Decorative Blocks | 300+ | Carved woodwork, fangxin, zhaotou, gutou, rafters, queti, chuihua, railings, roof charms, etc. |
| Furniture | 37 | Cabinets (with storage), tables, chairs (sittable), beds, screens, doors and windows, etc. |
| Materials & Items | 104 | Jade, magnesite, hematite, cobalt, porcelain, dye powders, templates, food, etc. |
| Crafting Recipes | 412 | Shaped crafting, stonecutting, smelting, blasting, smoking and smithing transform |
| Ore Generation | 4 types | Jade, magnesite, hematite (Overworld) and cobalt ore (Nether) |
| Mob Drops | 2 types | Sheep/goats/foxes/rabbits drop fur; hoglins/ravagers drop raw meat |
| Resource Pack Files | 733 | Models and textures |
| Localization | ZH/EN | 800+ translations for `zh_cn` and `en_us` |

## Project Structure

```
Ultramarine/
├── pack.yml                  # Pack metadata (author, version, namespace)
├── configuration/            # CraftEngine configurations
│   ├── blocks/               # Blocks (building, roof tiles, carved elements, etc.)
│   ├── furniture/            # Furniture (with storage and interactive behaviors)
│   ├── material.yml          # Materials and items
│   ├── recipes.yml           # Crafting recipes
│   ├── categories.yml        # Categories
│   ├── lang.yml              # Translations
│   ├── image.yml             # Images
│   ├── settings.yml          # Ore generation and mob drops
│   └── templates/            # Templates
└── resourcepack/             # Models and textures
    └── assets/minecraft/
        ├── models/
        └── textures/
```

## Installation

1. Install [CraftEngine](https://github.com/Xiao-MoMi/craft-engine) on your server (check its [official documentation](https://xiao-momi.github.io/craft-engine-wiki/) for version requirements).
2. Place the entire `Ultramarine` folder from this repository into `plugins/CraftEngine/resources/`.
3. Run `/ce reload all` to reload CraftEngine.
4. Done.

## Credits

- [Ultramarine](https://github.com/LocusAzzurro/Ultramarine): Original author LocusAzzurro and contributors. All textures, models and gameplay designs come from the original mod.
- [CraftEngine](https://github.com/Xiao-MoMi/craft-engine): The server-side custom content engine by XiaoMoMi.

## License

- This project's code and configuration (CraftEngine configs, etc.) are licensed under the **MIT** License, see [LICENSE](LICENSE).
- The art assets (models and textures under `Ultramarine/resourcepack/`) come from the original mod and are licensed under **CC BY-NC 4.0 (Attribution-NonCommercial)**, see [resourcepack/LICENSE](Ultramarine/resourcepack/LICENSE).
- The original mod's code is licensed under BSD-3-Clause. This project is a **non-commercial** port for learning and exchange only; keep the original author's attribution when using or redistributing it.
