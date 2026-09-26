# Green Grow — SPEC

## Design rules (always)
- Designed with a neurodivergent young person.
- Clean screens, few elements.
- No flashing, no loud sounds, no sudden movements.
- Every change is explained in one or two simple, literal sentences.

## Concept
- The player grows plants and also does other farm jobs, like watering or selling crops.
- The player harvests plants when they are ready, then the cycle starts again.
- The player chooses where to place pots and plants in their garden.
- The player chooses seeds, sows them, watches them germinate, and moves them into pots or the ground as they grow.
- Inspired by Stardew Valley. It should feel relaxing. Based on an interest in horticulture, agriculture and gardening.

## Spec 1 · Story — Animal
- The player wants to raise animals and grow plants together on their farm.
- Plants die if the player forgets to water or feed them.
- There is no winning condition. The player can keep playing.

## Spec 2 · World — Forest
- The player's garden and animals are inside the forest.
- The forest has tall green trees, brown trunks and a dirt ground.
- Wild animals like deer and birds live in the forest with the player's animals.

## Spec 3 · Mechanics — Explore
- Plants grow to full size in 3 in-game days.
- Plants turn brown after 3 days, then die on day 4.
- The player can place plants anywhere in the forest space.

## How to work
1. Specs live in this file.
2. The game is built in separate modules (story, world, mechanics) so one can change without breaking the others.
3. All mechanics numbers (speeds, amounts, points) live together in one place (`CONFIG` in `index.html`).
4. Anything marked "(to be decided)" gets a simple suggestion, and we ask before deciding.
5. Build in small steps. Show each step and wait before going further.
6. After every change, check the game still matches this file.

## Decisions (made in step 2, the user said Claude could choose)
- "Brown after 3 days" means 3 days **without water**. Day 4 without water = the plant dies.
- A plant grows only when it had water in the last day. Water once a day → full size in 3 days.
- "Water or feed": plants get water, animals get feed. Hungry animals do not die. They just stop giving eggs or milk.
- Plant stages: seed → sprout (germinated) → young → growing → full size (ready to pick).
- A plant with leaves can be dug up with the Hand and moved into a pot or the ground.
- Seeds: carrot, tomato, sunflower. Farm animals: chicken (eggs), goat (milk).
- Farm jobs: sow, water, fill the can at the pond, harvest, feed animals, collect eggs and milk, sell at the shop.
- Wild deer and birds wander slowly in the forest. Birds fly slowly and land gently.
- Time stops while a card (welcome or shop) is open. One day = 2 real minutes.
- The farm is saved in the browser. The "?" button can start a new farm.
- No sound at all.

## Progress
- Step 1: the character walks in the forest. ✔
- Step 2: plants, pots, watering, harvest, shop, animals, wild animals, days, saving. ✔
