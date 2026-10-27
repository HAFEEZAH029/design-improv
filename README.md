# Start.ng “Surprise me” picker

This project is a standalone concept for one small component that can sit inside Start.ng’s existing game discovery area. It is not a replacement homepage and it does not add a new game to the platform.

## What it does

- Shows a stack of real Start.ng games on the front and behind cards.
- Fans the cards out with a small bounce when the component appears.
- On **Surprise me**, shuffles the stack open into a V and closes it twice.
- Reveals a randomly selected game, its creator, and a link to play it.
- Supports narrow screens, keyboard focus, and reduced-motion preferences.

The prototype is in [index.html](./index.html). It uses plain HTML, CSS, and JavaScript, so it can be previewed by opening that file in a browser. No packages or build step are required.

## How it fits into Start.ng

The picker is designed to occupy one card-sized slot in the existing **Games from the community** grid. The surrounding homepage keeps its current navigation, section headings, footer, and layout. The picker brings its own card content and interaction, then returns to the normal game grid beside it.

Its visual styling follows the current page’s light cream background, dark text, lime accent, fine borders, rounded corners, and compact button treatment. When merged into the platform, those prototype values should use Start.ng’s existing design tokens and shared card/button styles.

## Integration notes

1. Place the picker component in the existing games grid, where it will render as one card among the game cards.
2. Replace the prototype’s local `games` array in `index.html` with the games already supplied to that page by Start.ng. The selected item should include its title, creator, cover or illustration, and existing play URL.
3. Use the platform’s existing route helper or game URL when setting the **Play this game** link.
4. Keep the picker’s random selection client-side. It does not need its own API, account flow, leaderboard, or game session.
5. Keep the reduced-motion behavior and keyboard-accessible buttons when moving the markup and styles into the platform’s component system.

The current list of games and their links is sample prototype data so the interaction can be previewed independently. It should be connected to Start.ng’s live game data during integration.
