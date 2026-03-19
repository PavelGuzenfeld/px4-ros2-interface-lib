# Upstream Contribution Plan

> **DO NOT PR this file to upstream (Auterion/px4-ros2-interface-lib).**
> This is a local tracking document for the fork only.

Last updated: 2026-03-20

Upstream: https://github.com/Auterion/px4-ros2-interface-lib
Fork: https://github.com/PavelGuzenfeld/px4-ros2-interface-lib

---

## Already Merged Upstream

| Branch | PR | Status |
|---|---|---|
| `feat/home-position-setter-108` | [#189](https://github.com/Auterion/px4-ros2-interface-lib/pull/189) | MERGED |
| `fix/map-projection-prefix-152` | [#188](https://github.com/Auterion/px4-ros2-interface-lib/pull/188) | MERGED |
| `fix/vtol-status-timeout` | [#186](https://github.com/Auterion/px4-ros2-interface-lib/pull/186) | MERGED |

**Action:** Clean up these local branches — they can be deleted from the fork.

---

## Open PR

| Branch | PR | Status |
|---|---|---|
| `refactor/mode-executor-use-vehicle-command-sender` | [#192](https://github.com/Auterion/px4-ros2-interface-lib/pull/192) | OPEN |

---

## To Contribute — Substantive Features

### Priority 1: Small / Easy PRs

| Branch | Commits | Description | Notes |
|---|---|---|---|
| `single_compatibility_check_backport_1.6.1` | 1 | Only call `messageCompatibilityCheck` once | Clean single commit, easy review |
| `rm-local-position-msg-check` | 2 | Remove local position & manual control message checks | Small cleanup |
| `python-pre-commit` | 1 | Add Black to pre-commit for Python formatting | Tooling improvement |

### Priority 2: Feature Additions

| Branch | Commits | Description | Notes |
|---|---|---|---|
| `autonomous_acro` | 3 | Builder pattern for mode Settings, `prevent_arming` flag, acro yaw control, autonomous power loop example | Self-contained feature |
| `cruise_control_mode` | 2 | New cruise control mode with diff-drive setpoint type | Rover feature |
| `manual_rover_control_mode` | 3 | Manual rover control (includes cruise_control commits) | Depends on cruise_control_mode |

### Priority 3: Large Feature (needs rebase/cleanup)

| Branch | Commits | Description | Notes |
|---|---|---|---|
| `feat/enable-flight-modes-to-keep-alive-on-fmu-conn-loss` | 15 | FW control API, lateral/longitudinal control setpoints, keep-alive on FMU connection loss | **Main branch** — `feat/fw-ctrl-and-flight-mode-keep-alive` (7 commits) is an older subset. Contribute only this one. Needs rebase on upstream/main and likely squash into logical commits. |

### Priority 4: Needs Evaluation

| Branch | Commits | Description | Notes |
|---|---|---|---|
| `modify-executor-commandsync-function` | 1 (+ 2 version fixes) | Don't pass executor ID if not in charge yet | Check if still relevant after #192 merges |

---

## Not Contributing (CI / Test / WIP / Stale)

| Branch | Reason |
|---|---|
| `buidljet` | CI infra (buildjet runners), typo in name |
| `fix-ci` | CI fixes, partially superseded by upstream |
| `release/1.16` | Release branch CI tweak |
| `release/1.5.1` | Release branch CI tweak |
| `hackathon` | Experimental |
| `prerelease/0.0.200` | Test release |
| `test/0.0.0` | Test release |
| `test_build` | Test build |
| `interrupting-executor-example` | WIP |
| `test-BodyframeDynamicSetpoint-requirements` | WIP testing |
| `0.0.3-message-fix` | Old message removal, likely stale |

**Action:** Consider deleting these from the fork after confirming nothing valuable remains.
