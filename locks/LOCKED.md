> **Experimental. We are just trying this.** [Disclaimer](../DISCLAIMER.md) · Kaspa Testnet-10 only. tKAS has no value.

# Lock (pre-run 38)

Locked before the first submit.

- Network: Testnet-10. The desk node is not restarted and it is not stopped.
- One knob: ready cap 32. Thirty chains are available, so the cap does not hold a chain back. The rate stays 460 sompi per gram. No second lane. No fee climb. No payment ladder. The chain count is not raised.
- The lane submits only to the desk node. While it is on, it slows other users' low-fee transactions on our node.
- No coin join in this run. At 2026-11-14T16:40:24Z the payment pile had 195 coins at or above 10 tKAS, together 4,753 tKAS. That covers the same fee cap pre-run 37 hit. Value is not moved onto the funding key.
- No covenant families, no mint line, no guest. The funding key was at 17,905 usable tKAS at 2026-11-14T15:49:57Z, under the 18,000 line. Pre-run 36 and pre-run 37 did not spend it.
- The two keys this series leaves unused stay unused. The lane spends the payment pile.
- One counter: the desk node. The Mini is not reachable. No Mini-armed file.
- Fee cap 3,000 tKAS, moved cap 4,000 tKAS, pile floor 200 tKAS. Same guards as pre-run 37.
- Disk line: abort if the desk is under 150 GB free. It was 328.21 GB at 2026-11-14T16:40:24Z.
- A miss is a retry with the fix written first. This page is not rewritten to match the result.
