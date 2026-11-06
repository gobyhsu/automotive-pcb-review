---
name: automotive-pcb-review
description: Review 12 V and 24 V automotive power and protection PCB schematics, layouts, and prototype readiness. Use for reverse battery, overcurrent, transient immunity, EMC layout, thermal, and fabrication reviews.
---

# Automotive PCB review

Review the identified revision. Record available schematic, routed board or Gerbers, BOM, harness, enclosure, customer requirements and test results. Inspect read-only by default. For an authorized layout revision, preserve the baseline and re-export affected manufacturing files.

1. Define the boundary. Record supply and load envelopes, startup, chassis and signal returns, backfeeds, upstream fuse, and accessible reset. Clarify whether a current limit means a timed trip threshold or an instantaneous ceiling.
2. Trace actual copper and components for normal, reverse, short and transient states. Locate paths using reference designators, PCB layers and coordinates. With only a schematic, mark layout findings as pending. Use [power protection](references/power-protection.md).
3. Compare credible coincident pin and device stresses to exact vendor data, including temperature, tolerances, and waveform. Treat calculated scenarios, measurements and missing evidence separately.
4. Match trace/space, copper thickness, drills and mask to the chosen fabrication process. Reconcile BOM, placement and polarity. Check assembly risk at vias in solder pads and exposed pads. Record ERC/DRC separately from electrical behavior.
5. Report priority, revision/location, observation, evidence status, consequence, proposed correction and closure test. Distinguish checks blocking prototype work from those blocking release.

Use [standards and evidence](references/standards-and-evidence.md) to define applicable test requirements. Start bench validation with a current-limited supply. Progress to the real load, harness, enclosure and applicable transient/EMC tests. Log source settings, probe points, waveforms, trip, and reset.
