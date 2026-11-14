> **Experimental. We are just trying this.** [Disclaimer](../DISCLAIMER.md) · This page does not start a machine. Pre-run 38. Not Wednesday. Not Tuesday. Not pre-run 1 to 37.

# Targets

Pre-run 37 scored ready cap 16 on a quiet desk mempool. The lane's own log sat at 16 pending and 420–449 submit-OK a minute. The probe's template median stayed one heavy transaction, and ready-mass medians were 4.43–8.55 blocks. The fee cap of 3,000 tKAS stopped new submits inside the sixth minute. The next single knob is the ready cap, now 32.

**Question.** On our desk node, with thirty of our heavy chains available and the rate held, what does a ready cap of 32 do to the template and the fee estimate, against a no-lane baseline in the same run?

Thirty chains and a cap of 32 means the cap does not hold a chain back. Pre-run 36 and pre-run 37 set the cap under the chain count, at 8 and at 16, and the lane's pending sat on that cap. This run moves the cap to the other side of the chain count. We do not also change how many chains exist. That would be a second knob.

**Target.** The lane runs only in the middle step and is at zero at the end. A table, written after the tail from this run's own files, shows template storage mass, template transaction count, ready mass, and the fee estimate, for the baseline minutes, the ready-cap-32 minutes, and the return minutes. **Met means the table exists and the lane is at zero, not that a particular theory won.** If the fee cap stops new submits before the six minutes are up, the table still counts. The minutes after that stop are what the logs show.

## Why the twelve families are not in this run

At 2026-11-14T15:49:57Z the funding key's usable balance (coins over 3 tKAS, above that line) was 17,905 tKAS. Pre-run 36 and pre-run 37 did not spend that key. A family window aborts under 18,000 tKAS. This run does not start the families, the mint line, or the guest. The two keys this series leaves unused stay unused.

## The pile, read before the arm

The lane takes a coin only when that coin is at or above 10 tKAS. At 2026-11-14T16:40:24Z the payment pile had 195 such coins, together 4,753 tKAS. Pre-run 37 moved 3,099.63 tKAS before its fee cap. This pile covers that same cap. This run does not join coins. Value stays where it is. Nothing moves onto the funding key.

## The one change, written before the arm

**Ready cap 32.** Our heavy lane (the same shape as pre-run 37: one input, two outputs, storage mass about 266,666, submitted only to the desk's private node). Thirty chains are available. The ready cap is 32, which is above that chain count. The rate is 460 sompi per gram, held. No second lane. No climb toward 1,405 or 2,000. The fee cap stays 3,000 tKAS. The moved cap stays 4,000 tKAS. The pile floor stays 200 tKAS. Those three guards are the same as pre-run 37. None of them is the knob.

**While it runs it slows other users' low-fee transactions on our node. We say so here, in public.**

| Order | Step | Lane | Length |
|---:|---|---|---:|
| 1 | BASE | off (N=0, ready cap 0) | 3 whole minutes |
| 2 | HOLD | N=30, ready cap 32, rate 460 | 6 whole minutes |
| 3 | RETURN | off | 3 whole minutes |

The desk node is not restarted. One counter: the desk. The Mini is not reachable. No payment flood. No heavy submit to a public node.

Disk line: abort if the desk is under 150 GB free.
