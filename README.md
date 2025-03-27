# Delta Dore

This a *custom component* for [Home Assistant](https://www.home-assistant.io/).

The `Delta Dore Tydom` integration allows you to observe and control [Delta Dore Tydom smart home gateway](https://www.deltadore.fr/).

This integration can work in local mode or cloud mode depending on how the integration is configured (see Configuration part)
The Delta Dore gateway can be detected using dhcp discovery.

![GitHub release](https://img.shields.io/github/release/CyrilP/hass-deltadore-tydom-component)
[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg)](https://github.com/hacs/integration)

**This integration will set up the following platforms.**

Platform | Description
-- | --
`binary_sensor` | Show something `True` or `False`.
`sensor` | Show info.
`switch` | Switch something `True` or `False`.
`cover` | controls an opening or cover.
`climate` | controls temperature, humidity, or fans.
`light` | controls a light.
`lock` | controls a lock.
`alarm_control_panel` | controls an alarm.
`update` | firmware update

**This integration has been tested with the following hardware.**

- Cover (Up/Down/Stop)
- Tywatt 5400, Tywatt 1000
- Tyxal+ DFR
- K-Line DVI (windows, door)
- Typass ATL (zones temperatures, target temperature, mode (Auto mode is used for antifrost), water/heat power usage) with Tybox 5101
- Calybox
- Tyxal+, Tyxal CSX40
- TYXIA 6610
- BSO
- Naviclim Atlantic 875311
- RF 6600 FP : partial issue #92

Some other functions may also work or only report attributes.

## Configuration is done in the UI

<!---->
The hostname/ip can be :
* The hostname/ip of your Tydom (local mode only). An access to the cloud is done to retrieve the Tydom credentials
* mediation.tydom.com. Using this configuration makes the integration work through the cloud

The Mac address is the Mac of you Tydom

Email/Password are you Dela Dore credentials

The alarm PIN is optional and used to set your alarm mode
