# AUTODOZER

A personal mobile robotics concept exploring a compact platform for light material-moving tasks.

**Status: concept and design documentation.** The requirements below are design targets. This repository does not yet provide validated controls software, a complete electrical design, or a tested autonomous robot.

## Design brief

| Item | Current design direction |
| --- | --- |
| Base | Approximately 24 × 24 inch frame |
| Initial mobility | Wheeled platform; tracks are a possible later iteration |
| Candidate drive hardware | Repurposed mobility motors |
| Candidate controller | Arduino-based control experiments; final architecture undecided |
| Intended terrain | Snow, gravel, dirt, and sand; capability remains unverified |
| Tooling | Blade and actuator integration under consideration |

## Engineering questions

1. What wheel diameter, reduction ratio, mass, and traction are needed for the target load?
2. Should each side share a mechanical drive or use independent motors?
3. What operating voltage and current limits suit the selected motors, controller, and battery?
4. How will steering, braking, loss of communication, and emergency stop behavior be verified?
5. What mechanical loads will the blade and actuator transmit into the frame?

Motor ratings and catalog estimates are inputs to design calculations, not measured platform performance. Final parts selection requires verified specifications and bench measurements.

## Proposed validation sequence

- **Requirements:** define load, speed, runtime, grade, and stopping criteria.
- **Bench:** characterize the drive and actuator subsystems separately with bounded current and motion.
- **Manual control:** verify command limits, stop behavior, and communication-loss handling.
- **Mobility:** record traction, steering, current draw, and temperature under controlled conditions.
- **Task testing:** evaluate material-moving behavior only after subsystem checks pass.

These are planned checks; none is marked as passed here.

## Documentation to accompany an implementation

Publish the reviewed bill of materials, block diagram, wiring, configuration, control logic, and test records with the corresponding source revision. Identify unresolved assumptions and operating limits.

No autonomous-operation or payload claims are made at this stage.

See the [portfolio documentation standards](https://github.com/jackjavo826-source/jackjavo826-source/blob/main/PORTFOLIO_STANDARDS.md).
