# Third-party notices

## LibreHardwareMonitor

TH Suite (Hardware module) uses the **LibreHardwareMonitorLib** NuGet package to read hardware sensors.

- Project: https://github.com/LibreHardwareMonitor/LibreHardwareMonitor
- License: Mozilla Public License 2.0 (MPL-2.0) — https://www.mozilla.org/MPL/2.0/

The library is used unmodified, as a NuGet dependency. Its source code is available at the project page above.

## PawnIO

Low-level hardware access (CPU temperature, motherboard sensors, fan control) relies on the **PawnIO** driver, which is installed separately by the user (for example with `winget install PawnIO`). TH Suite does not bundle or redistribute the driver.

- Project: https://github.com/namazso/PawnIO.Setup
