# Rock Go Crunch — Beta 1.0

**Rock Go Crunch** is a mobile-first browser game about mining, prospecting, processing minerals, completing a geology museum, and gradually automating the work you have already mastered.

The core loop is simple: **dig → discover → process → donate or sell → upgrade → go deeper**.

The mine is intentionally a fictional composite mine. Mineral names, chemistry, processing relationships, and museum facts are grounded in real geology and gemology, but the game does not pretend that every included material would naturally occur together in one real deposit.

## Beta 1.0

Beta 1.0 marks the point where the main gameplay loop is considered stable enough for broader playtesting. The focus now shifts toward pacing, balance, content length, clarity, and polish.

Changes from v3.1 include:

- **Beta 1.0** branding throughout the game
- a quieter **Auto-process** control moved to the bottom of each expanded Workbench card
- a public-facing README focused on the game rather than repository setup
- the v3.1 mastery, museum, Sell All, scanner, and visual-readability improvements carried forward unchanged

## Mining and prospecting

Each rock face is a 10×10 grid containing isolated finds, small veins, large veins, fossils, and historical artifacts.

Mining is not completely blind. Some rock faces contain subtle geological tells that suggest promising places to begin. The scanner adds a second layer of prospecting:

- each scan covers a 3×3 area
- scanned tiles stay marked for the current rock face
- overlapping scans accumulate
- a hidden occupied tile scanned twice gains a very faint generic density anomaly
- the anomaly does not reveal the identity or colour of the hidden find
- early scanner levels report chemistry or mineral-family information
- later scanner upgrades provide more precise identification
- additional upgrades increase scans per rock face

Pick durability and scanner uses reset whenever a fresh rock face is started. There are no real-time energy timers.

## Museum and mastery

The museum is the collection heart of the game. Minerals and ores have visible specimen slots, with facts displayed directly beneath each collected form.

For processable minerals, the usual collection path is:

**Raw → Tumbled → Cut**

Ores use a simpler natural-ore → refined-metal relationship.

Completing every museum specimen for a material gives that material a gilded mastery state, reveals a bonus discovery fact, and unlocks **Auto-process** for that material. Automation is earned one collection at a time.

Mastered minerals and ores are also eligible for the Workbench **Sell All** action. Unmastered materials, fossils, and historical artifacts are left untouched, so bulk selling grows naturally as the museum fills.

## Current mine depths

### Depth 1 — Upper Seam

- Quartz
- Amethyst
- Hematite → Iron
- Chalcopyrite → Copper
- rare Trilobite fossil
- rare Mining Tag artifact

### Depth 2 — Lower Works

Earlier finds continue at different rates, with:

- Garnet
- Topaz
- Pyrite

### Depth 3 — Deep Gallery

Earlier finds continue alongside:

- Citrine
- Calcite
- Fluorite
- Aquamarine
- Sapphire
- Cassiterite → Tin
- Ammonite fossil
- Old Mining Lamp artifact

## Visual language

Related minerals deliberately share visual relationships. Quartz, Amethyst, and Citrine use the same basic crystal silhouette with different colours because they are quartz varieties. Other minerals, ores, fossils, and artifacts use more distinct silhouettes and palettes so they remain readable at small sizes.

A full custom sprite-art pass is planned for a later major version.

## Game philosophy

Rock Go Crunch borrows the satisfying progression structure of incremental and mobile games without pay-to-win mechanics.

- one in-game currency
- no premium currency
- no real-money purchases
- no energy timers
- no pay-to-skip
- processing itself is free
- better equipment and automation are earned through play
- deeper does not automatically mean "better"; earlier materials remain relevant

Progress is saved locally in the browser.
