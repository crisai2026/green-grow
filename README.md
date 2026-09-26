# Green Grow

A calm farming game inside a forest. Grow plants from seeds, water them, harvest them and sell them. Raise chickens and goats. Deer and birds live in the forest too.

The game is designed with a neurodivergent young person: clean screens, few elements, no flashing, no sound and no sudden movements.

## How to play

Open `index.html` in any web browser. There is nothing to install.

- Walk: arrow keys or W A S D, or click where you want to go.
- Tools: keys 1 to 5 (Hand, Water, Seeds, Pot, Feed). Click something, or press Space.
- Plants need water once a day. After 3 days they are full size.
- A plant with no water for 3 days turns brown. On day 4 it dies.
- Feed animals once a day to get eggs and milk.
- Sell your basket at the shop. Fill your watering can at the pond.

## Files

- `index.html` - the whole game (one file, no dependencies).
- `SPEC.md` - the design specification and the decisions made.

## Changing the game

All the numbers (speeds, prices, days) are in `CONFIG` at the top of `index.html`. All the words are in `Story`. The code is split into modules: Story, World, Mechanics, UI and Game.
