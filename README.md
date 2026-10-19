# Pokémon Living Dex Tracker

A free, fan-made Living Pokédex tracker for **20 Pokémon games across Generations I–V**. Find out where to obtain each Pokémon, how to evolve or breed it, when trading is required, and how many copies to collect to maintain a complete Living Dex.

**This is an unofficial, noncommercial community project.** It is not affiliated with or endorsed by Nintendo, Game Freak, or The Pokémon Company.

## Features

- **20 supported games**, from Pokémon Red and Blue through Black 2 and White 2.
- **Game-specific checklists** with separate completion progress for each title.
- **Acquisition guidance** covering wild encounters, gifts, special encounters, evolutions, breeding, trading, and Pokémon unavailable in the selected game.
- **Locations, encounter levels, encounter odds, and alternative routes** where provided by the game's data.
- **Living Dex copy counts** to help you retain each Pokémon while evolving or breeding additional specimens.
- **Search and filtering** by Pokémon name, National Dex number, route, game, region, and acquisition method; optionally hide completed entries.
- **Era-specific Pokémon sprites** displayed for each game, with fallback imagery where available.
- **Progress bar**, favorites for game selection, and light/dark themes.
- **Animated Poké Ball checkboxes** and optional synthesized catch sounds, with reduced-motion support.
- **Automatic local progress saving** in your browser. Optional Claude-account synchronization is supported when running inside a compatible Claude artifact environment.
- **Responsive layout** for desktop and mobile browsers.

## Supported games

| Generation | Games |
| --- | --- |
| I | Red, Blue, Yellow |
| II | Gold, Silver, Crystal |
| III | Ruby, Sapphire, FireRed, LeafGreen, Emerald |
| IV | Diamond, Pearl, Platinum, HeartGold, SoulSilver |
| V | Black, White, Black 2, White 2 |

## Getting started

The application is supplied as a self-contained **`index.html`** file. Its HTML, CSS, JavaScript, and Pokédex data are embedded in that file; no package manager, build step, or server-side application is required.

1. Download or clone this repository.
2. Open `index.html` in a modern browser, or serve the folder with any static web server.
3. Choose a game and mark Pokémon as obtained using the Poké Ball controls.

Internet access is needed to load externally hosted sprites and Google Fonts. The Pokédex data itself is embedded in the page.

## Publishing as a website

For a static host such as **Netlify**, upload the folder containing `index.html`, or connect your repository for deployment. No build command is necessary. On **GitHub Pages**, publish the branch containing `index.html`. **Vercel** can also serve the project as a static website.

> **Important:** On a standalone website, progress is stored in that browser's `localStorage`. Claude-specific account sync uses the `window.claude` integration and should not be expected to work on an independent host without implementing a separate backend and authentication system.

## How to use

1. **Select a game** from the game navigation; favorite games you use often.
2. **Find Pokémon** by searching for names, numbers, locations, or game references.
3. **Filter the list** by region or acquisition method, or hide already caught Pokémon.
4. **Read the acquisition instructions** for the selected game, including alternatives and trade requirements.
5. **Track copies** when additional Pokémon are required for your Living Dex.
6. **Mark a Pokémon as collected** by selecting its Poké Ball. Your progress is saved automatically on the current browser/device.

Different games maintain separate checklists. Clearing browser storage, using a private window, or moving to a different device may cause locally stored progress to be unavailable.

## Data and image credits

The application includes per-game source links in its **Sources** menu and additional acquisition notes in its footer. Refer to those links for source details and caveats. Sources referenced in the application include:

- [PokéAPI](https://pokeapi.co/) and its [Pokémon sprites repository](https://github.com/PokeAPI/sprites)
- [pret](https://github.com/pret) game-data and disassembly projects
- [Serebii](https://www.serebii.net/)
- Additional game-specific references listed directly in the website

The sprites are **loaded from the PokéAPI sprites GitHub repository**, rather than included as image files in this project. Access to those files does not itself grant a license to redistribute Pokémon artwork.

## Accuracy and limitations

The tracker aims to provide a practical acquisition route for each applicable Pokédex entry. Certain Pokémon may require other games, special events, multiple systems, trading, or transfer features. Encounter rates and routes may depend on game-specific conditions. Review the selected game's notes, source links, and the footer for important exceptions.

Game data and acquisition guidance should be considered a community reference and may need corrections. Report inaccuracies with the **game, Pokémon, location, and a supporting source**.

## Contributing

Suggestions, issue reports, accessibility improvements, and corrections are welcome. When proposing a data correction, include the affected game and National Dex entry, the current displayed information, the proposed correction, and a verifiable source.

## Technology

- HTML5, CSS, and vanilla JavaScript
- Embedded JSON datasets for individual games
- Browser `localStorage` for local progress
- Optional Claude artifact APIs for account synchronization within Claude
- Externally hosted sprites and fonts

No React, Node.js, external database, or compilation step is required for basic standalone hosting.

## Disclaimer and rights

Pokémon and associated character names, game titles, and artwork belong to their respective rights holders, including Nintendo, Game Freak, and The Pokémon Company. This project is an unofficial fan-made community tool created for informational and personal collection-tracking purposes. It is not affiliated with, sponsored by, or endorsed by those companies.

The project is intended to be free and noncommercial. **Noncommercial status does not automatically grant permission to use copyrighted material.** Review relevant rights-holder policies and applicable licenses before distributing assets or republishing third-party content.

No open-source license for the website's original code is asserted by this README. Add a `LICENSE` file if you decide to grant reuse permissions for your own contributions; any such license cannot grant rights to third-party Pokémon imagery or trademarks.

---

*Built with the help of Claude.*
