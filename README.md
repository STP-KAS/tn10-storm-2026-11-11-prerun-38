> **Experimental. We are just trying this.** [Disclaimer](DISCLAIMER.md) · Kaspa Testnet-10 only; tKAS has no value.
>
> **This is a pre-run. Pre-run 38.** It is not the Wednesday run. It is not the Tuesday run. It is not pre-run 1 to 37, and it does not edit their repos. A read does not start a runner.

# tn10-storm-2026-11-11-prerun-38

**Pre-run 38: one heavy lane of ours, ready cap 32, on the desk node, with the lane off at both ends.** The neuron stays [tn10-storm-2026-11-11](https://github.com/STP-KAS/tn10-storm-2026-11-11). This repo does not edit that repo.

> **Our own testing.** This is our own Kaspa Testnet-10 testing, run on our own machines and nodes. What these pages report is what we observed in this run; it is not a claim of how TN10 or Kaspa behave in general.

| Field | Value |
|---|---|
| Target | A table of the desk template and the desk fee estimate with our lane off, then at ready cap 32, then off again. The lane returns to zero |
| The change | One knob: the ready cap, set at 32. Thirty chains are available, so a cap of 32 does not hold a chain back. The rate stays 460 sompi per gram. No payment ladder. No second lane. No fee climb |
| Met or not met | **met** on the table and on the lane returning to zero. BASE 16:43–16:45Z: fee estimate 100 / 100 / 100, lane submit 0. HOLD: the lane log shows pending 30, not 32, and submit-OK 501, 530, 532 and 540. In the twelve samples from 16:46:17Z through 16:50:22Z the template's heavy count is 1, template storage mass 266,694–269,119, our heavy class 18–28 at fee rate 460, and 56–576 other transactions sit in the 101–149 fee band. Ready mass in those samples is 17.06–25.72 blocks. The fee cap stopped new submits at 16:50:39Z (350 submit-OK in that minute, fees 3,010.67 tKAS). The one sample over 400,000 is 465,835 at 16:50:43Z, classed other, after our heavy class had gone. RETURN fee estimate 100 / 100 / 100, pending 0 from 16:52. 2,453 submit-OK, 0 rejects |
| Retry count | 0. The next attempt is a new repo. This one is not resumed |
| Core tags | — |
| Status | done. Closed from the lane log and the probe |

Plan, lock, and the prediction are in [plan/PLAN.md](plan/PLAN.md), [locks/LOCKED.md](locks/LOCKED.md), and [plan/PREDICTIONS.md](plan/PREDICTIONS.md). Written before any submit.

While the lane is on, it slows other users' low-fee transactions on our node. We say so here.
