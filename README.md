# nicFW880 Greek Amateur Radio Frequency List

Clean amateur-radio channel list for **nicFW880 v5 BETA 7** / Radtel RT-880 family.

## Files

- `channels.csv` — ready-to-import channel list.
- `group.csv` — group definitions used by `channels.csv`.

## Channel order

1. SV1 repeaters — ordered approximately by distance from Piraeus
2. SV3 repeaters — ordered approximately by distance from Piraeus
3. SV8 repeaters — ordered approximately by distance from Piraeus
4. SV9 repeaters — ordered approximately by distance from Piraeus
5. UHF cross-band links
6. Greek beacons — nationwide, nearest first
7. Selected active European 29 MHz repeaters
8. Amateur satellites
9. Calling, FT8 and APRS channels

Only amateur-radio frequencies are retained. PMR/FRS/GMRS, CB, airband, public-service,
military/SATCOM and other non-amateur entries from the original 999-channel file were removed.

Digital-only DMR/D-STAR repeaters are not included because this list is intended for direct
analogue operation with nicFW880.

## Important UHF links

- `LINK SV8M Naxos` — **438.925 MHz**, CTCSS **107.2 Hz** (Ymittos link to SV8M/R4b Naxos)
- `LINK SV8U Argol` — **430.225 MHz**, CTCSS **71.9 Hz**
- `LINK SV8U Thira` — **430.125 MHz**, CTCSS **71.9 Hz**
- `LINK SV8U Amorg` — **430.325 MHz**, CTCSS **71.9 Hz**
- `LINK R0 Lamia` — **430.875 MHz**, CTCSS **82.5 Hz**

The current RAAG UHF link set is also included.

## 29 MHz / 10 m

The old Greek SV1K 29.660 MHz entry was not included because current repeater listings mark it
off-air. The list instead contains selected currently operational European repeaters on RH1-RH8
(29.620-29.690 MHz), useful during Sporadic-E and other 10 m openings.

## Beacons

Greek beacons are programmed receive-only (`TX_Power=N/T`) to prevent accidental transmission.
They are ordered approximately by great-circle distance from Piraeus.

## SHF / 23 cm

No 23 cm repeater memory is included. The RT-880 receiver covers 18-620 MHz and 840-1000 MHz,
so the Greek 1.2 GHz / 23 cm repeaters (for example 1298 MHz) are outside the radio's RF range.
Adding them to the codeplug would therefore create unusable memories.

## Sources / verification

Checked 2026-09-06 against:

- Radio Amateur Association of Greece (RAAG) repeater/link tables
- RepeaterBook Greece and European 10 m listings
- ERDYP repeater/beacon information
- G0LGS IARU Region 1 beacon lists
- UK Repeater 10 m list
- Dodecanese Radio Amateur Association beacon information
- Existing user channel list, with duplicates and invalid/non-amateur entries removed

`R0b Milos` is retained as an on-air override based on a recent successful local contact even
though some online directories still show an older off-air status.

## Notes

Repeater receive tone decoding is left open (`RX_Tone=None`) while the required access tone is
stored in `TX_Tone`. This avoids losing a repeater whose output does not transmit CTCSS while
still keying it correctly.

Pure beacon channels and satellite beacon/SSDV receive channels are set to `N/T`.
