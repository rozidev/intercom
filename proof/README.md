# Proof Artifacts

Run date: 2026-02-24 17:11:44 +07:00

Fork URL: https://github.com/rozidev/intercom
Selected app profile id: lane_board
Selected app label: Intercom Delivery Lane Board
Selected naming mode: semantic
Selected proof style: tx_sim_focus
Mutating command: seal_delivery_lane_lane
Query command: review_delivery_lane_lane
Payout Trac address: trac1hzds4d5l8nvcm0wxurga9f59xzu6e2pjkakaprxaqu43h6z3444q6af5vg

Rationale: This run differs via semantic naming pair (seal/review_*) plus tx-simulation focused proof artifacts.

## Files
- run.log: pear runtime startup capture (sanitized).
- run-screenshot.png: visual render of run.log.
- command-mapping.log: protocol mapTxCommand output for selected command pair.
- tx-sim.log: simulation command string and preflight mapping evidence.

## Commands used
- pear run . --peer-store-name proof-lane --msb-store-name proof-lane-msb --subnet-channel proof-delivery-board --dht-bootstrap 127.0.0.1:49737 --sidechannels proof-lane-room
- /tx --command '{"op":"seal_delivery_lane_lane","status":"MVP ready","note":"competition-proof"}' --sim 1
- /tx --command "review_delivery_lane_lane"
