# 🇬🇷 nicFW880 Greek Amateur Radio Frequency List

A clean, practical amateur-radio memory set for **nicFW880 v5 BETA 7** and the **Radtel RT-880 / iRadio 880 family**, built around operation from **Piraeus / Attica**.

The aim is simple: keep the memories that are actually useful to a Greek radio amateur, remove non-amateur clutter, and put repeaters in an order that makes sense on the radio rather than in a random database dump.

## 📦 Files

| File | Purpose |
|---|---|
| [`channels.csv`](channels.csv) | Main nicFW880 channel list — **157 memories** |
| [`group.csv`](group.csv) | Group definitions used by the channel list |

## 🗺️ Memory order

The list is arranged deliberately:

1. **SV1 repeaters** — approximately nearest to Piraeus first
2. **SV3 repeaters**
3. **SV8 repeaters**
4. **SV9 repeaters**
5. **UHF repeater links / cross-links**
6. **Greek amateur beacons** — nationwide, approximately nearest to Piraeus first
7. **Selected European 29 MHz / 10 m repeaters** useful during Sporadic-E and other openings
8. **Amateur satellites**
9. **Calling, FT8 and APRS memories**

The main repeater memories use short radio-friendly names such as `R2b Ymittos`, `RU1 Ymittos`, `R4b Naxos` and `RS2 Ymittos`.

## 📡 Bands included

- 10 m
- 6 m
- 4 m
- 2 m
- 70 cm
- **23 cm / 1.2 GHz**
- Amateur satellite uplinks/downlinks that fit the radio
- Greek amateur beacon frequencies

### 23 cm / SHF

The list includes the analogue **SV1W / RS2 Ymittos** repeater:

- **RX:** 1298.050 MHz
- **TX:** 1270.050 MHz
- **CTCSS:** 94.8 Hz

nicFW880 BETA 7 provides radio-side **Band Plan editing**. Actual usable RF coverage still depends on the particular radio, hardware and calibration, so users should verify operation on their own unit before transmitting.

## 🔗 Important UHF links

The long-distance UHF links were intentionally retained instead of being removed by the SV1/SV3/SV8/SV9 geographic filter.

| Memory | Frequency | CTCSS |
|---|---:|---:|
| `LINK SV8M Naxos` | **438.925 MHz** | **107.2 Hz** |
| `LINK SV8U Thira` | 430.125 MHz | 71.9 Hz |
| `LINK SV8U Argol` | 430.225 MHz | 71.9 Hz |
| `LINK SV8U Amorg` | 430.325 MHz | 71.9 Hz |
| `LINK R0 Lamia` | 430.875 MHz | 82.5 Hz |
| `LINK R1 Sparti` | 430.800 MHz | 88.5 Hz |
| `LINK R3 Chania` | 430.825 MHz | 88.5 Hz |

The Naxos link is deliberately present as a first-class memory rather than being hidden inside a repeater note.

## 🌍 29 MHz / 10 m repeaters

Selected European **RH1–RH8** FM repeaters are included between **29.620 and 29.690 MHz**, with the usual -100 kHz inputs. These are intended for the days when 10 m opens and repeaters hundreds or thousands of kilometres away suddenly become workable.

The old Greek **SV1K / 29.660 MHz** memory is currently omitted because current public repeater listings mark it off-air.

## 🛰️ Satellites

The satellite section contains practical memories for satellites and spacecraft commonly used or monitored by radio amateurs, including ISS, SO-50, AO-91, PO-101, CAS-series satellites, RS-44, AO-123, AO-73 and related beacon channels.

Satellite beacon/telemetry-only memories are set **N/T** where appropriate to avoid accidental transmission.

## 📻 Beacons

Greek amateur beacons are retained **nationwide**, regardless of SV region, and are placed approximately by distance from Piraeus. Beacon memories are programmed receive-only (`TX_Power=N/T`).

## 🧹 What was removed

The source channel dump contained many entries that do not belong in a Greek amateur-radio memory list. This version removes:

- PMR / FRS / GMRS
- CB
- airband
- public-service and commercial frequencies
- military / non-amateur SATCOM
- duplicate or obviously broken entries
- frequencies outside the intended amateur allocations

Digital-only DMR/D-STAR repeaters are not the focus of this list; it is primarily an **analogue nicFW880 operating list**.

## ⚙️ nicFW880 notes

- Built for **nicFW880 v5 BETA 7** CSV structure.
- `RX_Tone=None` is normally left open on analogue repeaters while the required access tone is stored in `TX_Tone`.
- Beacon and telemetry-only memories use `N/T` where appropriate.
- `group.csv` separates geographic repeater groups, links, beacons, 10 m, satellites and operating channels.

## 🔎 Sources and verification

Last reviewed: **2026-09-07**.

Useful sources used to cross-check the list include:

- [Radio Amateur Association of Greece (RAAG / ΕΕΡ)](https://raag.org/)
- [RepeaterBook — Greece](https://www.repeaterbook.com/row_repeaters/index2.php?state_id=GR)
- [Σύλλογος Ελλήνων Ραδιοερασιτεχνών — HAG](https://hag.gr/portal/)
- IARU Region 1 beacon information and national beacon lists
- Published Greek repeater/link information
- Real-world operating reports where current directory data conflicts with observed operation

`R0b Milos` is intentionally retained because it has been successfully worked recently from Piraeus despite older directory information showing a different status.

## ⚠️ Operating note

Repeater status, tones and links can change without notice. Always comply with the current Greek amateur-radio band plan and licence conditions, and verify questionable entries before transmitting.

---

**73 de SV1EEX**
