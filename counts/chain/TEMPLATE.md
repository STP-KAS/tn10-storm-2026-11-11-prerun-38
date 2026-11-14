> **Experimental. We are just trying this.** [Disclaimer](../../DISCLAIMER.md) · Kaspa Testnet-10 only. tKAS has no value. Counts only.

# Template, pre-run 38

The desk probe, every 20 s, on our own desk node. A cell is the median of that minute's samples. Where a minute has two samples, the median is the average of the two. Template storage mass is the mass the template's transactions carry. "Under 400k" is how many of those samples had template storage mass under 400,000. The lane log is a different clock: its pending count is the lane's own in-flight count at the minute line. "Our heavy" is the probe's class for ids this lane had already written, at fee rate 460.

The lane was off in BASE (16:43–16:45Z) and RETURN (16:52–16:54Z). HOLD on the clock was 16:46–16:51Z, ready cap 32, thirty chains available, rate 460. The fee cap stopped new submits at 16:50:39Z. The 16:51 minute is still inside that clock, and the lane submitted 0 in it.

| Minute (UTC) | Step | Samples | Mempool | Ready count | Ready mass, blocks of 500k | Template txs | Template storage mass | Samples under 400k | Fee estimate priority / normal / low | Our heavy in mempool | Lane pending | Lane submit-OK |
|---|---|---:|---:|---:|---:|---:|---:|---:|---|---:|---:|---:|
| 2026-11-14T16:43 | BASE | 3 | 0 | 0 | 0 | 0 | 0 | 3 of 3 | 100 / 100 / 100 | 0 | 0 | 0 |
| 2026-11-14T16:44 | BASE | 3 | 0 | 0 | 0 | 0 | 0 | 3 of 3 | 100 / 100 / 100 | 0 | 0 | 0 |
| 2026-11-14T16:45 | BASE | 3 | 0 | 0 | 0 | 0 | 0 | 3 of 3 | 100 / 100 / 100 | 0 | 0 | 0 |
| 2026-11-14T16:46 | HOLD | 3 | 529 | 529 | 17.50 | 3 | 266,718 | 3 of 3 | 435.67 / 184.35 / 114.47 | 25 | 30 | 501 |
| 2026-11-14T16:47 | HOLD | 3 | 431 | 431 | 21.77 | 4 | 266,750 | 3 of 3 | 439.42 / 184.56 / 114.49 | 24 | 30 | 530 |
| 2026-11-14T16:48 | HOLD | 2 | 370 | 370 | 18.12 | 5.5 | 266,757 | 2 of 2 | 411.07 / 182.83 / 114.35 | 18.5 | 30 | 532 |
| 2026-11-14T16:49 | HOLD | 3 | 346 | 346 | 20.37 | 4 | 266,726 | 3 of 3 | 429.70 / 184.01 / 114.44 | 24 | 30 | 540 |
| 2026-11-14T16:50 | HOLD | 3 | 294 | 344 | 20.69 | 4 | 269,119 | 2 of 3 | 441.93 / 184.70 / 114.50 | 19 | 0 | 350 |
| 2026-11-14T16:51 | HOLD | 3 | 0 | 0 | 0 | 0 | 0 | 3 of 3 | 100 / 100 / 100 | 0 | 0 | 0 |
| 2026-11-14T16:52 | RETURN | 3 | 0 | 0 | 0 | 0 | 0 | 3 of 3 | 100 / 100 / 100 | 0 | 0 | 0 |
| 2026-11-14T16:53 | RETURN | 3 | 0 | 0 | 0 | 0 | 0 | 3 of 3 | 100 / 100 / 100 | 0 | 0 | 0 |
| 2026-11-14T16:54 | RETURN | 3 | 0 | 0 | 0 | 0 | 0 | 3 of 3 | 100 / 100 / 100 | 0 | — | — |

Across the twelve samples from 16:46:17Z through 16:50:22Z, while our heavy class was present, template storage mass runs from 266,694 to 269,119. All twelve are under 400,000. The template's own heavy count is 1 in each of those twelve. Our heavy class in those samples is 18 to 28 transactions, all ready, fee rate 460 on the class. The same samples also hold other transactions: 56 to 576 of them sit in the 101–149 fee band. Mempool size in those samples is 110 to 631.

The one HOLD sample at or above 400,000 is 465,835, four transactions over 100,000 storage mass, at 16:50:43Z. That sample is after the fee cap. Our heavy class is 0. The four are classed other, and the fee estimate is 100 / 100 / 100. Ready mass in the twelve samples above runs from 17.06 to 25.72 blocks. The 16:51 samples are empty.

The lane's own minute lines say pending 30 and submit-OK 501, 530, 532 and 540. Thirty chains exist, so pending did not reach 32. The 16:45 row stamps `ready_cap` 32 on the first tick of 16:46, and that minute has 0 submits. The 16:50 row stamps pending 0 on the first tick of 16:51, after the cap at 16:50:39Z, and that minute has 350 submits. The 16:51 row stamps `ready_cap` 0 on the first tick of 16:52. The submit count is the minute. The 16:54 lane minute was not flushed. The probe covers it, and the end line says pending 0.

The lane's end line at 16:55:00Z: 2,453 submit-OK, 0 rejects, 0 lost, fees 3,010.67 tKAS, parked 91.99 tKAS, 90 coins taken, pending 0. Node rate on the lane's own entries was 459.99–460. Storage mass did not drift. The second lane submitted 0.

One BASE sample, at 16:43:55Z, read mempool size 0 and 10 other transactions, template storage mass 1,157. One BASE sample, at 16:45:57Z, read mempool size 8, template storage mass 322,375, one transaction over 100,000 storage mass, classed other, not our heavy. The lane submitted 0 in both minutes, and the fee estimate is 100 / 100 / 100. One RETURN sample, at 16:54:28Z, read mempool size 0 and 58 other transactions, template storage mass 750, in the 101–149 fee band. We report the size field and the entry read as they are.
