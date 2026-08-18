# WOB 1.2.2(1) — Full Changelog

**Tracked 1.1 baseline:** `WOB for gpt(2).txt (tracked 1.1 baseline)`  
**Previous design checkpoint:** `WOB 1.2.1(5).txt`  
**Patch base:** `WOB 1.2.2.txt`  
**Current:** `WOB 1.2.2(1).txt`  

## Headline KPIs

- **149** substantive matched-card changes from the tracked 1.1 baseline.
- **10 added / 10 removed or exported / 5 recognized renames**.
- **116** pure card-number shifts tracked separately.
- **13** substantive main-card records changed from 1.2.1(5) → 1.2.2(1).
- Latest 1.2.2 → 1.2.2(1) patch: **6 content/metadata records + 2 number-only records**.
- **7** critical functional/text flags remain before freeze.

## 1.2.2 → 1.2.2(1) patch

- **Citadel's Longsword:** Agreed fix applied: rarity common → uncommon after removing the free body.
- **Hoarder's Might:** Partial wording repair; still needs “remove a hoard counter from it.”
- **Plains1:** Basic-land metadata normalized to “basic land”; numbering shifted into 290–293.
- **Plains2:** Basic-land metadata normalized to “basic land”; numbering shifted into 290–293.
- **Plains3:** Basic-land metadata normalized to “basic land”; numbering shifted into 290–293.
- **Unfatomable pact:** Partial typo repair; still needs “If X is 10 or greater.”
- **Sylvine Grove:** card number 291 → 288.
- **Terraforming Expanse:** card number 292 → 289.

## Important audit correction

- **Scrapfang, Clever Saboteur:** the previous “undefined X” functional flag was a false positive and is closed. The X construction itself is left untouched; only the separate `onto the battlefield` wording cleanup remains.

## What went well

- UR noncreature now has a common payoff at the correct point in the curve: Stormborn Drake moved to 3U 1/3 while retaining double prowess.
- WU artifact animation now exists at common through Field Mender, giving a clear progression into Argent-Wind Artisan and Ingvar.
- BR signaling is materially cleaner: Marcelus is 1BR instead of triple hybrid, and Steppe Errand-Runner no longer self-supplies a Resource or triggers repeatedly in one turn.
- Hoard thresholds read more intentionally: Steppe Lancer’s 3-counter threshold can no longer be bypassed by targeting itself, while Sparks moved from an unrealistic 6 to a reachable 4.
- Food/Resource burst and old Alimancy dependency were reduced: Dealer now makes only a Resource, and cumulative Food-only sacrifice text fell sharply from baseline.
- Green interaction was simplified without deleting green’s Hoard identity: Brawl and Sylvine Ambush stopped being incidental Hoard producers.
- Artifact/Equipment density stayed stable while colored Equipment distribution became more deliberate, preserving cross-archetype glue without overloading colorless picks.
- All ten Limited archetypes now have a viable C/U skeleton. The set has crossed from 'theoretical skeleton repair' into 'playtest and cleanup' territory.
- The follow-up 1.2.2(1) file actually applies the agreed Citadel’s Longsword uncommon shift and normalizes all 20 basic lands to the same metadata convention.
- Scrapfang’s X construction is no longer treated as a functional error in the audit; only its independent 'onto the battlefield' wording cleanup remains.

## What remains

- Finish the seven genuinely critical text fixes: Hoarder’s Might, Cruel Bargain, Unfatomable pact, Karra’s Battle Rage, Argent-Wind Defender, Beckanham, and Defend the Gates. Hoarder’s Might and Unfatomable pact were partially edited in 1.2.2(1) but still need one word-level correction.
- Resolve high-priority clarity/intent flags such as Steppe Lancer’s 3+ threshold wording, Council’s Mortuary’s trigger window, Unskilled Concoctioner’s activation window, Boreal Mirror’s target wording, and Steel-Paws’s combat-damage wording.
- Do not add more archetype support on theory alone. Run Draftmancer/Cockatrice and track seatability, common pick rates, win rates, game length, and signpost dependence.
- Watch—not preemptively nerf—Field Mender, Citadel’s Extractor and Slumbering Beetle. They are the clearest current candidates for data-driven balance follow-up.
- Finish the remaining typo/flavor cleanup after functional fixes. The typo sheet preserves voice/slang where possible and focuses suggestions on actual grammar/meaning problems.

## Rarity distribution

| Rarity | 1.1 | 1.2.1(5) | 1.2.2(1) | Δ 1.1→current |
|---|---:|---:|---:|---:|
| Common | 107 | 109 | 108 | +1 |
| Uncommon | 92 | 85 | 86 | -6 |
| Rare | 70 | 79 | 79 | +9 |
| Mythic | 20 | 16 | 16 | -4 |

## Limited status

- **GU — Hoard / counters / move counters:** READY. No structural change before playtest.
- **WB — Sacrifice / 1/1s / small recursion:** READY — text cleanup. Fix Beckanham self-name and clarify Mortuary once-per-turn window.
- **UB — Artifacts / graveyard / surveil:** READY — critical text fix. Define X on Scrapfang before freeze.
- **BG — Death drain / graveyard / reanimate:** READY. No skeleton change; test reanimation pace.
- **RW — Auras / Equipment:** READY — pending rarity edit. Apply Citadel's Longsword uncommon rarity as agreed.
- **BR — Artifact sacrifice / menace / accumulation:** READY. Marcelus 1BR and Errand changes fixed signaling/engine issues.
- **RG — Power matters / large creatures:** READY — text cleanup. Fix Steel-Paws wording; no skeleton redesign.
- **WU — Artifact animation:** READY — fixed in 1.2.2. Field Mender closes the missing common animation rung. Watch 4/4 repeatability in playtest.
- **UR — Noncreature / prowess:** READY — fixed in 1.2.2. Stormborn now lets the deck advertise itself at common.
- **GW — Creatures / go-wide / Hoard:** READY. No structural change before playtest.

## Next phase

After the seven critical text fixes and the selected high-priority clarity checks, freeze the theoretical skeleton and move to Draftmancer/Cockatrice. Measure archetype seatability, common pick rates, game length, signpost dependence, and the watchlist cards before doing another balance pass.
