# Upstream Contribution Plan

> **DO NOT PR this file to upstream (Auterion/px4-ros2-interface-lib).**
> This is a local tracking document for the fork only.

Last updated: 2026-03-20

Upstream: https://github.com/Auterion/px4-ros2-interface-lib
Fork: https://github.com/PavelGuzenfeld/px4-ros2-interface-lib

---

## Already Merged Upstream (branches deleted from fork)

| Branch | PR |
|---|---|
| `feat/home-position-setter-108` | [#189](https://github.com/Auterion/px4-ros2-interface-lib/pull/189) |
| `fix/map-projection-prefix-152` | [#188](https://github.com/Auterion/px4-ros2-interface-lib/pull/188) |
| `fix/vtol-status-timeout` | [#186](https://github.com/Auterion/px4-ros2-interface-lib/pull/186) |
| `single_compatibility_check_backport_1.6.1` | Already upstream (Beat Küng's commit `84b863e`), branch deleted |

---

## Open PR (your work)

| Branch | PR | CI | Review |
|---|---|---|---|
| `refactor/mode-executor-use-vehicle-command-sender` | [#192](https://github.com/Auterion/px4-ros2-interface-lib/pull/192) | All green | Awaiting maintainer review |

---

## Other People's Branches on Fork (not your commits)

These branches live on the fork but contain commits by Auterion employees, not by you.
They should be cleaned up (deleted) from the fork.

| Branch | Author | Notes |
|---|---|---|
| `autonomous_acro` | Auterion | Builder pattern, acro mode |
| `cruise_control_mode` | Auterion | Cruise control + diff-drive |
| `manual_rover_control_mode` | Auterion | Rover control (includes cruise_control) |
| `feat/enable-flight-modes-to-keep-alive-on-fmu-conn-loss` | Auterion | FW control API + keep-alive |
| `feat/fw-ctrl-and-flight-mode-keep-alive` | Auterion | Older subset of above |
| `rm-local-position-msg-check` | bertug@auterion.com | Message check removal |
| `python-pre-commit` | guillaume | Add Black pre-commit |
| `modify-executor-commandsync-function` | Auterion | Executor ID fix |
| `buidljet` | Auterion | CI runners |
| `fix-ci` | Auterion | CI fixes |
| `release/1.16` | Auterion | Release branch |
| `release/1.5.1` | Auterion | Release branch |
| `hackathon` | Auterion | Experimental |
| `prerelease/0.0.200` | Auterion | Test release |
| `test/0.0.0` | Auterion | Test release |
| `test_build` | Auterion | Test build |
| `interrupting-executor-example` | Auterion | WIP |
| `test-BodyframeDynamicSetpoint-requirements` | Auterion | WIP testing |
| `0.0.3-message-fix` | Auterion | Old message removal |
