# Equipment plan: what to buy, why, and what it costs

> Written 1 October 2026. Prices are a snapshot for that date, not a promise.
> Rate used: **1 USD = 11 819 UZS** (source: open.er-api.com, updated
> 1 October 2026). A month from now everything will be cheaper or dearer.

## How to read the prices here

Every price carries one of three labels. The difference between "verified" and
"estimate" is the difference between a plan and a fantasy.

| Label | Meaning |
|---|---|
| **verified** | price found in a specific shop, link given |
| **estimate** | order of magnitude known, but confirm before buying |
| **not stocked** | checked, absent from the Tashkent shop |

We do not invent prices. Where it says "estimate", go and check — it takes
five minutes.

---

## Tier 1. First workbench

Goal: build and program something that shows numbers.

| Item | UZS | In USD | Status |
|---|---|---|---|
| ESP32 DevKit v1 (USB-C) | 97 000 | ~$8.20 | **verified**, Uzum |
| Breadboard 830 point | 25 000 | ~$2.10 | **estimate** |
| Dupont wires (set) | 20 000 | ~$1.70 | **estimate** |
| LEDs and resistors | 15 000 | ~$1.30 | **estimate** |
| **Total** | **~157 000** | **~$13.30** | |

Alternative: a ready ESP32 Basic Starter Kit with breadboard, wires, LEDs,
DHT11, OLED, relay and PIR — **200 000 UZS (~$17)**, **verified**, OLX Tashkent.
43 thousand more, but everything arrives at once in one case.

**Recommendation:** for the first session, take the kit. Sourcing parts one by
one is organiser work, not beginner work on a first evening. Break the kit down
as the number of participants grows.

---

## Tier 2. Ordinary electronics and embedded

| Item | UZS | In USD | Status |
|---|---|---|---|
| ESP32-S3-DevKitC-1 v1.1 | 80 000 | ~$6.80 | **verified**, Microelectronica, Tashkent |
| Digital multimeter, basic | 120 000 | ~$10.20 | **estimate** |
| Logic analyser, 8 channel | 90 000 | ~$7.60 | **estimate**, usually AliExpress |
| Soldering station 60 W | 350 000 | ~$29.60 | **estimate** |
| Enclosure | 25 000 | ~$2.10 | **estimate** |
| **Total** | **~665 000** | **~$56.30** | |

**What is genuinely needed.** A multimeter — yes, without it you cannot tell
whether a circuit works. A soldering station — **not for the first session**,
only when a project appears that cannot be done on a breadboard.

**What you can skip.** An oscilloscope. For a while it will sit unused while
costing as much as the other five items combined. If a project appears where it
is unavoidable, we will discuss it then.

---

## Tier 3. Air sensor — the first real project

This is the project we proposed as the through-line: embedded → MQTT → HTTP API
→ storage → dashboard. It answers a real city problem, not an exercise one.

| Item | UZS | In USD | Status |
|---|---|---|---|
| PM2.5 sensor SDS011 (UART) | 350 000 | ~$29.60 | **estimate**, AliExpress |
| ESP32-S3 or DevKit v1 | 80 000 | ~$6.80 | **verified** |
| Ventilated enclosure | 60 000 | ~$5.10 | **estimate** |
| 5 V power supply | 40 000 | ~$3.40 | **estimate** |
| Wires, connectors | 35 000 | ~$3.00 | **estimate** |
| **Total** | **~565 000** | **~$48** | |

**Verified and important:** the SDS011 is **not stocked** at the Tashkent
electronics shop (checked 1 October 2026). So the sensor ships from AliExpress —
allow 2–3 weeks for delivery and customs. The ESP32 board, meanwhile, is
available in the city today.

**The main caveat.** The SDS011 is an optical sensor: it reacts to humidity and
to dust, not to PM2.5 alone. For a learning project that is fine, but **you
must not publish its readings as "air quality in Tashkent."** That would be a
lie you would later have to retract. As a measuring instrument for comparison
"before and after" at one spot, it works.

---

## Tools: what to buy and what not to

**Buy first:**

| Tool | Why |
|---|---|
| Multimeter | the only tool needed all the time |
| Screwdriver set | small thing, but you stop without it |
| Tweezers | to hold small parts |
| Crimping tool | for Dupont wires and terminals |

**Do not buy until needed:**

- an oscilloscope — expensive and idle;
- a hot air rework station — a third of a board will not need it;
- a 3D printer — one of the most expensive investments, not needed before the
  first enclosure;
- a 50-part "electronics for beginners" kit — half of it will never be used.

---

## Where to buy

**Verified sources in Uzbekistan:**

| Shop | What | Link |
|---|---|---|
| Microelectronica, Tashkent | ESP32-S3, components | [electron.uz](https://electron.uz/) |
| Uzum | ESP32 DevKit, general | [uzum.uz](https://uzum.uz/) |
| OLX Uzbekistan | ready kits, used hardware | [olx.uz](https://www.olx.uz/) |

**AliExpress** — for everything not in the city: logic analyser, soldering
stations, the SDS011. One honest downside: 2–3 weeks shipping plus customs.

**Used and OLX** — for anything needed "to try it out". A soldering station at
half price in good condition is normal practice, not an admission.

---

## What to buy in multiples

| Item | How many | Why |
|---|---|---|
| ESP32 board | one per participant | everyone builds their own; shared hardware teaches waiting |
| Breadboard wires | ×1.5 per participant | they get lost and torn, factually |
| Multimeter | 2–3 per group | everyone will want it at once |
| Power supply | 1–2 per group | no need to share, but you need a spare |

---

## Order of purchase when money is tight

1. **Nothing.** The learning track runs in a browser and needs no hardware.
   That is not an excuse, it is a fact: the first two levels require nothing
   bought.
2. **An ESP32 kit (~200 000 UZS)** — when the first person wants to build
   something physical.
3. **Multimeter plus a couple of boards** — when there is more than one
   participant.
4. **The PM2.5 sensor** — when someone is ready to carry the project through to
   a dashboard.

Buying everything at once is a mistake. Unused hardware teaches nobody, and
the community budget is spent for nothing.

---

## What this plan does not solve

- **No justification of why the community needs it.** Hardware without a task
  is a warehouse. Every item above must answer "which lab does this serve".
- **No storage plan.** A community workshop needs space, inventory and
  someone responsible. Without that, there is nothing to buy.
- **No running costs.** Power, shipping, replacing what breaks.
- **Nothing about electrical safety.** If a project involving mains voltage
  appears, that is a separate document with separate requirements.

## When this plan goes stale

The prices here are a snapshot from 1 October 2026. In three months they will
be cold. What needs rechecking is not the whole file but three things: board
prices, whether the SDS011 is in the city, and the dollar rate.