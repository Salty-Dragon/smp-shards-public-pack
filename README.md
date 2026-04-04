# SMP Shards Public Pack

A Minecraft resource pack for version 1.21.11 that adds custom items using the `custom_model_data` system. This pack provides custom models and textures for shard items, mythic items, and other special items used on the server.

## How It Works

Custom items are defined by overriding vanilla item models with `range_dispatch` entries that map `custom_model_data` values to custom models. Each base item type (e.g., Nether Star, Heart of the Sea, Shield) has its own dispatcher file in `assets/minecraft/items/`.

## Custom Items

### Nether Star Items (Base Item: Nether Star)

| CMD ID | Item Name        | Model                    |
|--------|------------------|--------------------------|
| 1001   | Echo Shard       | `shards/echo_shard`      |
| 1002   | Health Shard     | `shards/health_shard`    |
| 1003   | Lightning Shard  | `shards/lightning_shard` |
| 1004   | Hell Shard       | `shards/hell_shard`      |
| 1005   | Sky Shard        | `shards/sky_shard`       |
| 1006   | Ice Shard        | `shards/ice_shard`       |
| 1007   | Shadow Shard     | `shards/shadow_shard`    |
| 1008   | Nature Shard     | `shards/nature_shard`    |
| 1009   | Earth Shard      | `shards/earth_shard`     |
| 1010   | Celestial Shard  | `shards/celestial_shard` |
| 1011   | Void Shard       | `shards/void_shard`      |
| 1012   | Time Shard       | `shards/time_shard`      |
| 1013   | Chaos Shard      | `shards/chaos_shard`     |
| 1014   | Upgrade Shard    | `shards/upgrade_shard`   |
| 1015   | Reroller Shard   | `shards/reroller_shard`  |
| 1016   | Repair Kit       | `shards/repair_kit`      |

### Heart of the Sea Items (Base Item: Heart of the Sea)

| CMD ID | Item Name  | Model                |
|--------|------------|----------------------|
| 2001   | Extra Life | `shards/extra_life`  |

### Shield Items (Base Item: Shield)

| CMD ID | Item Name       | Model                              |
|--------|-----------------|------------------------------------|
| 1017   | Beserker Shield | Vanilla shield (model and texture) |

## Adding a New Item

1. **Choose a base item** and assign a unique `custom_model_data` ID.
2. **Create a model JSON** in `assets/minecraft/models/item/shards/` (if using a custom model).
3. **Add a texture PNG** in `assets/minecraft/textures/item/` (if using a custom texture).
4. **Add a dispatcher entry** in the corresponding `assets/minecraft/items/<base_item>.json` file with the new CMD ID threshold.

## Installation

Place this pack in your Minecraft `resourcepacks` folder and enable it in-game.
