# Start.ng Games page concept

This is a visual mockup of Start.ng’s **All games from the community** page, with the **Surprise me** game picker placed in the first slot of the existing game grid. It demonstrates how the component fits alongside the platform’s search, category tiles, filters, and game cards. It is a concept preview, not a replacement homepage or a game published to Start.ng.

## The picker

- Starts with a real community game on the front ticket and two other game tickets stacked behind it.
- Floats gently in the game grid, pausing while hovered or focused.
- On the visitor’s first scroll, a small gift follows a steady curved path from beside the Start.ng logo to the picker. A long dashed lime trail follows and gradually clears behind it; at the card edge, the gift bursts into confetti and reveals a briefly tilted “Arcade makes the choice” label.
- Fans the smaller tickets into place with a bounce as the page loads.
- On **Surprise me**, cycles through games while the stack opens into a V and closes twice.
- Reveals the selected game, creator, and play link in the card.
- Supports responsive layout, keyboard focus, and reduced-motion preferences.

## Preview

Open [index.html](./index.html) in a browser. It uses plain HTML, CSS, and JavaScript, with no packages or build step. The search field also filters the sample game cards by title and creator.

## Fit with Start.ng

The mockup follows the Games page structure and styling shown in the current platform: centered page width, cream background, dark text, lime accent, rounded category tiles, filter pills, and four-column game cards. The picker uses the same card dimensions, border, cover area, title and creator hierarchy, and bottom action row. In the real page, it would be rendered as one item in the existing game-card grid; the platform’s header, footer, filters, and other sections would remain in place.

For a production merge, replace the prototype game array with the Games page’s existing game data and use its cover images and URL/routing helpers. Reuse the platform’s design tokens and existing game-card styles. The picker only needs the game list already available to that page; it does not require a new API, account flow, leaderboard, or game session.

Category and game-cover artwork in this mockup is simplified concept art to represent the surrounding page layout. The game names, creators, and routes in the picker are sample entries and should be connected to the live game data when integrated.
