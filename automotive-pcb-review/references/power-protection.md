# Power protection and layout

- Trace reverse-battery and short-circuit paths through MOSFET body diodes, TVS, chassis bonds and auxiliary wiring. For a latched cutoff, verify the actual device variant, reset threshold and whether stored charge or backfeed prevents power cycling. Fuse selectivity needs the real time-current curve and fault-source impedance.
- Treat raw-input alarm taps as their own branch. Inspect protection placement, short-to-chassis on each lead, isolation, strain relief and false triggering from negative pulses. Raw taps ahead of the switch require independent branch protection.
- For TVS, use standoff, actual pulse current, source impedance, temperature and energy. Follow the connector-to-clamp outgoing and return paths, including bottlenecks and via transitions. Probe the protected pins as well as the TVS. During a negative pulse a held +30 V node and a −50 V input create an 80 V differential before overshoot. This synthetic scenario illustrates why both voltages must be considered together.
- Check startup and turn-off MOSFET SOA using the simultaneous VDS and current trajectory, pulse duration, temperature and repetition. Avalanche or pulsed current ratings provide different evidence. Flag operation outside the published SOA coverage.
- Trace Kelvin pickup at both shunt pads to the sense pins. Check shared copper with load, supply and decoupling paths. Budget threshold and delay using tolerances, sense error and pickup geometry. Verify normal operation and fault response across the intended conditions.
- Keep decoupling close to the actual supply and return pins. Inspect copper necks, ground return, vias and heating in the final enclosure. Use temperature-dependent I²R for an initial estimate and measure during the real duty cycle.
- Verify exact footprint and pad functions against vendor drawings. Check solder-paste openings and via-in-pad treatment with the assembler. Some exposed pads require isolation.

Example device reference: [TI LM749x0-Q1 data sheet](https://www.ti.com/lit/ds/symlink/lm74910-q1.pdf). Apply its limits to the matching device and revision.
