![ThymeWorld](images/logo.png)
# ThymeWorld

A random map generator for [Dominions 6](https://www.illwinter.com/dom6/index.html).
Generates balanced, wrapping maps with a surface and an underground plane for
any mix of land, sea and cave nations, then lets you inspect and tweak the
result in a built-in editor before exporting it to the game.

## Screenshots

<details>
<summary>Territory lens</summary>

![Territory view](images/thyme-world-territory.png)

</details>

<details>
<summary>Simple terrain lens</summary>

![Terrain view](images/thyme-world-terrain.png)

</details>

<details>
<summary>Generation settings</summary>

![Generate modal](images/thyme-world-generate-modal.png)

</details>

<details>
<summary>Balance stats</summary>

![Map statistics](images/thyme-world-stats.png)

</details>

## Download

Go to [Releases](https://github.com/DrThyme/ThymeWorld/releases) and download the latest version for your platform:

| Platform | File |
|----------|------|
| Windows  | `.msi` or `.exe` installer |
| macOS    | `.dmg` disk image |
| Linux    | `.AppImage` or `.deb` package |

## Usage

1. Launch ThymeWorld.
2. **Generate**: pick the player count (or a disciples team layout), a nation
   for each seat, terrain weights, and anything you want to change under
   *Advanced* (rivers, mountain passes, throne placement, how sea and cave
   nations are arranged, balance weights).
3. Inspect the map. Switch lenses, check the balance stats, click a province
   or a connection to edit it, jump between the surface and the underground.
   Don't like it? **Regenerate** rolls a fresh seed with the same settings.
4. **Export** to a folder of your choice. This writes `<Name>/<Name>.map`
   and `.d6m` (plus `_plane2` files for the underground). Put the `<Name>`
   folder in your Dominions 6 `maps` folder and the map shows up in-game.

## Features

**Balance**

- Balanced start placement: every nation gets a comparably sized homeland
  and comparable distances to its nearest rivals. The five fairness weights
  are adjustable.
- Rivers with bridges and mountain-pass ridges with gaps, placed by the
  balancer so no capital is walled in. Counts and lengths are configurable.
- Thrones: one per player two moves from its capital (default), or
  *contested* thrones on neutral ground between exactly two players.
- Maps for 3 to 50 players.

**Nations**

- Every base-game and Dominions Enhanced nation across all eras, with
  capital and cap-ring terrain matching each nation's needs. A OneAge list
  mixes eras.
- **Sea nations**: one shared ocean, a separate sea for each, or random
  pairs.
- **Cave nations**: a full underground plane with cave homelands, gates,
  and player-to-player tunnels. Cave nations that share a region meet
  through a seeded shape: a wide front, a chokepoint, two doors, a narrow
  corridor, or a hub with one central province for three or more.
- **Disciples games**: up to 8 teams of any sizes, teammates placed side by
  side and declared to the game.

**Editor**

- Lenses: the map drawn with the game's own artwork, a territory overlay,
  a teams overlay, or flat terrain colours. Overlays for connections,
  starts, thrones and gates.
- Edit any province's terrain and flags, any connection's type, on either
  plane.
- Balance statistics: homeland sizes, distance matrix, per-player terrain
  breakdown.

**General**

- Wrapping (toroidal) maps, 4800×3600 by default.
- Fully reproducible from a seed.
- Standalone desktop app for Windows, macOS and Linux.

## Not supported (yet)

- Non-wrapping maps.
- Editing province borders or moving capitals by hand; the editor changes
  terrain, flags and connections, not geometry.

## Contributors

- **Teju Jagua**
- **Selgeron**
- **Mechrite**

## Credits

- **Dominions 6: Rise of the Pantokrator** is made by
  [Illwinter Game Design](https://www.illwinter.com/). The terrain tiles and
  sprites used by the editor's game-art lens are Illwinter's artwork,
  bundled only so the editor can preview a map the way the game draws it.
- The game-art renderer is a port of
  [dom6-simple-map-editor](https://github.com/PKozdra/dom6-simple-map-editor)
  by PKozdra (MIT).

## AI Disclosure

This application was developed with the assistance of AI (Claude). The logo was also AI-generated.

## Bug Reports

Found a bug? [Open an issue](https://github.com/DrThyme/ThymeWorld/issues).
