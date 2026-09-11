---
navigation:
  icon: 'cropsnh:genericSeed:0:{crop:"cropsnh:corpseplant"}'
  title: The Graveyard Soil trick
  parent: /breeding.md
  position: 0
---

# The Graveyard Soil Trick

> [!TIP]
> **TL;DR.** Put **TiC Graveyard Soil** under your cross-crop and breed **Corium + Corium**.
> As of CropsNH 2.0.114 Corium is in three pools (`BROWN`, `COW`, `MUSHROOM`). Two members of
> that union need graveyard soil: **Corpseplant** and **Zomplant**. Everything else is
> soil-rejected. This is no longer a single-result filter and the old 46-minute table is stale.
> Use the [web calculator](https://crops-nh.netlify.app/calculator.html) for current odds.

<details>
<summary>What changed in 2.0.114</summary>

Corium left `SILK` and `TENDRILLY`. It now registers only to `brown`, `cow`, and `mushroom`
(`MutationLoader` 2.0.114). Same-species Corium+Corium still matches those three pools
(pool lookup does not dedupe). After the soil check on graveyard:

- Spreading always returns Corium, which wants farmland → tick wasted
- Pool members that want farmland / dirt-grass / mushroom / nether-mushroom / stone / netherrack / thaum logs → wasted
- **Corpseplant** and **Zomplant** both want graveyard and both sit in Corium's pool union → both can land

Do not use the old single-result 46 / 67 / 153 minute table.

</details>

> [!NOTE]
> The idea generalizes: any restrictive soil — or a buried block only one pool member accepts —
> turns a noisy pool roll into a much smaller set of legal results.
