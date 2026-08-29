# Germany’s plug-in balcony PV cap is 800 VA, not 800 Wp

**Author:** Balkonkraftwerkfinder editorial · **Retrieved:** 29 Aug 2026 · **Status:** AI-edited, editorially reviewed · Not legal advice.

Short answer: German simplified rules for plug-in balcony solar (Steckersolargerät) use **two** limits at once — module capacity **up to 2 kW installed** and inverter output **up to 800 volt-amperes**. Shops often print “800 W balcony power plant” as if watt-peak on the panel and VA on the inverter were the same number. They are not. The Bundesnetzagentur states the same split: max 2,000 W module power, 800 VA inverter power, and if several devices sit behind the **same** withdrawal point, you **add** them. Source: [BNetzA, Balkon-Solaranlagen](https://www.bundesnetzagentur.de/DE/Fachthemen/ElektrizitaetundGas/ErneuerbareEnergien/Solaranlagen/Balkon_table.html) (retrieved 29 Aug 2026).

This note is a technical reading of that split for developers, product people, and anyone parsing shop SKUs. It is not a buying guide and not legal advice.

## Why the units differ

| Quantity | What it measures | Simplified-rule ceiling (BNetzA) |
|---|---|---|
| Installed / module power | Panel rating, usually Wp | 2 kW total |
| Inverter output | AC output of the micro-inverter | 800 VA total |
| Several devices | Same withdrawal point | Both ceilings **summed** |

Watt-peak is a DC rating under standard test conditions. Volt-ampere on the inverter is the AC output the grid sees. A 2,000 Wp kit with an 800 VA inverter is a common shop bundle. That does **not** mean 2,000 W is exported. Export is capped by the inverter.

The software “throttle” in an app does not rewrite the nameplate. If the type plate says more than 800 VA, an in-app limit is a different claim.

## What product copy usually collapses

| Shop line | Technical reading |
|---|---|
| “800 Watt balcony kit” with no split | Law/admin practice splits 2 kW modules **and** 800 VA inverter |
| “2,000 Wp set = 2,000 W feed-in” | Feed-in is inverter-limited |
| “Two 800 VA kits on one meter, each under the cap” | BNetzA: sum behind the same withdrawal point |
| “Wp = VA” | Different physical quantities |

If you are building a comparison table or a SKU parser, store **two** fields. Do not fold them into one “watt” integer.

## Registration is not optional because the grid notice is simpler

BNetzA still points operators to the Marktstammdatenregister. Simplified grid connection does not mean “no register.” Walkthrough on our site (inner page, not the homepage): [Balkonkraftwerk Anmeldung 2026](https://balkonkraftwerkfinder.de/anmeldung).

Everyday 800 VA vs module Wp, in German, with the same split: [800-W-Regelung](https://balkonkraftwerkfinder.de/800w-regelung). Rough yield only, not a promise: [Rechner](https://balkonkraftwerkfinder.de/rechner). Sets without a “best of” badge: [Vergleich](https://balkonkraftwerkfinder.de/vergleich).

Primary official page for the two ceilings: [BNetzA, Balkon-Solaranlagen](https://www.bundesnetzagentur.de/DE/Fachthemen/ElektrizitaetundGas/ErneuerbareEnergien/Solaranlagen/Balkon_table.html) (retrieved 29 Aug 2026).

## Checklist for a listing or firmware note

1. Type plate on the inverter: maximum **VA**, not only an app slider.
2. Module sum: installed power ≤ 2 kW.
3. Second device on the same meter: add VA and kW; do not reset per device.
4. MaStR done even if the DSO must not demand an extra signup for this class.
5. Do not advertise “800 W in, 800 W out” unless you measured AC output.

## FAQ

**Can the module Wp exceed 800?**  
Yes, as long as **installed** module power stays within 2 kW total. 800 VA is the inverter ceiling.

**Is 800 W the same as 800 VA?**  
Shops say watt. The administrative split uses **volt-amperes** for the inverter. This page does not convert VA to W.

**Two 800 VA kits?**  
Behind one withdrawal point the sums count. Two full 800 VA inverters are 1,600 VA total.

**Sources (retrieved 29 Aug 2026):** Bundesnetzagentur, Balkon-Solaranlagen. Research note, not legal advice. AI-edited, editorially reviewed.
