# Shelly 1PM

## Overview

Monitoring of almost all values the Shelly 1PM reports, except external sensors since I don't own one of those.

It has a fixed update time of 60s for all values, which might not be enough for some usecases - feel free to adjust it.

## Author

Leonard Winck

## Zabbix version

This template is compatible with Zabbix 7.0 and later versions.

## Macros used

|Name|Description|Default|Type|
|----|-----------|-------|----|
|{$SHELLYPWD}|<p>Password for admin user, if present</p>|`****`|Secret macro|

## Template links

There are no template links in this template.

## Discovery rules

There are no discovery rules in this template.

## Items collected

|Name|Description|Type|Key and additional info|
|----|-----------|----|----|
|Status gatherer|<p>This gatherer gathers all the data for the different items from the Rest-API Interface of the Shelly device.</p>|`HTTP agent`|shelly1pm.status<p>Update: 1m</p>|
|Actions Skipped Count|<p>-</p>|`Dependent item`|shelly1pm.status.actions_stats.skipped<p>Update: 0</p>|
|Configuration Changed Count|<p>-</p>|`Dependent item`|shelly1pm.status.cfg_changed_cnt<p>Update: 0</p>|
|Cloud Connection State|<p>-</p>|`Dependent item`|shelly1pm.status.cloud.connected<p>Update: 0</p>|
|Cloud Configured State|<p>-</p>|`Dependent item`|shelly1pm.status.cloud.enabled<p>Update: 0</p>|
|Filesystem Free|<p>-</p>|`Dependent item`|shelly1pm.status.fs_free<p>Update: 0</p>|
|Filesystem Total|<p>-</p>|`Dependent item`|shelly1pm.status.fs_size<p>Update: 0</p>|
|Input Event|<p>-</p>|`Dependent item`|shelly1pm.status.inputs0.event<p>Update: 0</p>|
|Input Event Count|<p>-</p>|`Dependent item`|shelly1pm.status.inputs0.event_cnt<p>Update: 0</p>|
|Input State|<p>-</p>|`Dependent item`|shelly1pm.status.inputs0.input<p>Update: 0</p>|
|MAC Address|<p>-</p>|`Dependent item`|shelly1pm.status.mac<p>Update: 0</p>|
|Power Consumption (1m)|<p>-</p>|`Dependent item`|shelly1pm.status.meters0.counters0<p>Update: 0</p>|
|Meters Self-Check State|<p>-</p>|`Dependent item`|shelly1pm.status.meters0.is_valid<p>Update: 0</p>|
|Overpower Value|<p>-</p>|`Dependent item`|shelly1pm.status.meters0.overpower<p>Update: 0</p>|
|Current Power Consumption|<p>-</p>|`Dependent item`|shelly1pm.status.meters0.power<p>Update: 0</p>|
|Current Power Consumption Time|<p>-</p>|`Dependent item`|shelly1pm.status.meters0.timestamp<p>Update: 0</p>|
|Total Power Consumption|<p>-</p>|`Dependent item`|shelly1pm.status.meters0.total<p>Update: 0</p>|
|MQTT Connection State|<p>-</p>|`Dependent item`|shelly1pm.status.mqtt.connected<p>Update: 0</p>|
|Overheating State|<p>-</p>|`Dependent item`|shelly1pm.status.overtemperature<p>Update: 0</p>|
|Memory Free|<p>-</p>|`Dependent item`|shelly1pm.status.ram_free<p>Update: 0</p>|
|Memory Total|<p>-</p>|`Dependent item`|shelly1pm.status.ram_total<p>Update: 0</p>|
|Relay Timer State|<p>-</p>|`Dependent item`|shelly1pm.status.relays0.has_timer<p>Update: 0</p>|
|Relay State|<p>-</p>|`Dependent item`|shelly1pm.status.relays0.ison<p>Update: 0</p>|
|Relay Overpower State|<p>-</p>|`Dependent item`|shelly1pm.status.relays0.overpower<p>Update: 0</p>|
|Relay Last Command Source|<p>-</p>|`Dependent item`|shelly1pm.status.relays0.source<p>Update: 0</p>|
|Relay Timer Duration|<p>-</p>|`Dependent item`|shelly1pm.status.relays0.timer_duration<p>Update: 0</p>|
|Relay Timer Remaining|<p>-</p>|`Dependent item`|shelly1pm.status.relays0.timer_remaining<p>Update: 0</p>|
|Relay Timer Started|<p>-</p>|`Dependent item`|shelly1pm.status.relays0.timer_started<p>Update: 0</p>|
|Cloud Serial Number|<p>-</p>|`Dependent item`|shelly1pm.status.serial<p>Update: 0</p>|
|Temperature Status|<p>-</p>|`Dependent item`|shelly1pm.status.temperature_status<p>Update: 0</p>|
|Current Time|<p>-</p>|`Dependent item`|shelly1pm.status.time<p>Update: 0</p>|
|Temperature Self-Check State|<p>-</p>|`Dependent item`|shelly1pm.status.tmp.is_valid<p>Update: 0</p>|
|Current Temperature|<p>-</p>|`Dependent item`|shelly1pm.status.tmp.tC<p>Update: 0</p>|
|Current Unixtime|<p>-</p>|`Dependent item`|shelly1pm.status.unixtime<p>Update: 0</p>|
|Update Availability|<p>-</p>|`Dependent item`|shelly1pm.status.update.has_update<p>Update: 0</p>|
|New Version Available|<p>-</p>|`Dependent item`|shelly1pm.status.update.new_version<p>Update: 0</p>|
|Current Version|<p>-</p>|`Dependent item`|shelly1pm.status.update.old_version<p>Update: 0</p>|
|Update Status|<p>-</p>|`Dependent item`|shelly1pm.status.update.status<p>Update: 0</p>|
|Uptime|<p>-</p>|`Dependent item`|shelly1pm.status.uptime<p>Update: 0</p>|
|WiFi Connection State|<p>-</p>|`Dependent item`|shelly1pm.status.wifi_sta.connected<p>Update: 0</p>|
|WiFi IP|<p>-</p>|`Dependent item`|shelly1pm.status.wifi_sta.ip<p>Update: 0</p>|
|WiFi RSSI|<p>-</p>|`Dependent item`|shelly1pm.status.wifi_sta.rssi<p>Update: 0</p>|
|WiFi SSID|<p>-</p>|`Dependent item`|shelly1pm.status.wifi_sta.ssid<p>Update: 0</p>|

## Triggers

|Name|Description|Expression|Severity|Dependencies and additional info|
|----|-----------|----------|--------|--------------------------------|
|Shelly 1PM: No data received for >3m|<p>-</p>|`nodata(/Shelly-1PM/shelly1pm.status,180s)=1`|Warning|<p>Manual close: YES</p>|
|Shelly 1PM: At least one action has been skipped|<p>-</p>|`change(/Shelly-1PM/shelly1pm.status.actions_stats.skipped)>0`|Warning|<p>Manual close: YES</p>|
|Shelly 1PM: System configuration has been changed|<p>-</p>|`change(/Shelly-1PM/shelly1pm.status.cfg_changed_cnt)>0`|Info|<p>Manual close: YES</p>|
|Shelly 1PM: Cloud connection state has changed|<p>-</p>|`change(/Shelly-1PM/shelly1pm.status.cloud.connected)<>0`|Warning|<p>Manual close: YES</p>|
|Shelly 1PM: Cloud configuration has changed|<p>-</p>|`change(/Shelly-1PM/shelly1pm.status.cloud.enabled)<>0`|Info|<p>Manual close: YES</p>|
|Shelly 1PM: Input state has changed|<p>-</p>|`change(/Shelly-1PM/shelly1pm.status.inputs0.input)<>0`|Info|<p>Manual close: YES</p>|
|Shelly 1PM: Meters self-check is not ok|<p>-</p>|`last(/Shelly-1PM/shelly1pm.status.meters0.is_valid)<>0`|Warning|<p>-</p>|
|Shelly 1PM: MQTT connection state has changed|<p>-</p>|`change(/Shelly-1PM/shelly1pm.status.mqtt.connected)<>0`|Warning|<p>Manual close: YES</p>|
|Shelly 1PM: Overheating event has been detected|<p>-</p>|`last(/Shelly-1PM/shelly1pm.status.overtemperature)=1`|Disaster|<p>-</p>|
|Shelly 1PM: Relay state has changed|<p>-</p>|`change(/Shelly-1PM/shelly1pm.status.relays0.ison)<>0`|Warning|<p>Manual close: YES</p>|
|Shelly 1PM: Overpower event has been detected|<p>-</p>|`last(/Shelly-1PM/shelly1pm.status.relays0.overpower)=1`|Disaster|<p>-</p>|
|Shelly 1PM: Device temperature is high|<p>-</p>|`last(/Shelly-1PM/shelly1pm.status.temperature_status)=1`|Average|<p>-</p>|
|Shelly 1PM: Device temperature is very high|<p>-</p>|`last(/Shelly-1PM/shelly1pm.status.temperature_status)=2`|High|<p>-</p>|
|Shelly 1PM: Device temperature status is unknown|<p>-</p>|`last(/Shelly-1PM/shelly1pm.status.temperature_status)=3`|Warning|<p>-</p>|
|Shelly 1PM: Temperature self-check is not ok|<p>-</p>|`last(/Shelly-1PM/shelly1pm.status.tmp.is_valid)<>0`|Warning|<p>-</p>|
|Shelly 1PM: Time is out of sync|<p>-</p>|`fuzzytime(/Shelly-1PM/shelly1pm.status.unixtime,60s)=0`|Warning|<p>-</p>|
|Shelly 1PM: Update available|<p>-</p>|`last(/Shelly-1PM/shelly1pm.status.update.has_update)=1`|Info|<p>-</p>|
|Shelly 1PM: Version has changed|<p>-</p>|`change(/Shelly-1PM/shelly1pm.status.update.old_version)<>0`|Warning|<p>Manual close: YES</p>|
|Shelly 1PM: Device has been restarted (Uptime <10m)|<p>-</p>|`last(/Shelly-1PM/shelly1pm.status.uptime)<600`|Warning|<p>-</p>|
|Shelly 1PM: Filesystem usage >=80%|<p>-</p>|`last(/Shelly-1PM/shelly1pm.status.fs_free)>=last(/Shelly-1PM/shelly1pm.status.fs_size)*0.8 and last(/Shelly-1PM/shelly1pm.status.fs_free)<last(/Shelly-1PM/shelly1pm.status.fs_size)*0.9`|Warning|<p>-</p>|
|Shelly 1PM: Filesystem usage >=90%|<p>-</p>|`last(/Shelly-1PM/shelly1pm.status.fs_free)>=last(/Shelly-1PM/shelly1pm.status.fs_size)*0.9`|Average|<p>-</p>|
|Shelly 1PM: Memory usage >=80%|<p>-</p>|`last(/Shelly-1PM/shelly1pm.status.ram_free)>=last(/Shelly-1PM/shelly1pm.status.ram_total)*0.8 and last(/Shelly-1PM/shelly1pm.status.ram_free)<last(/Shelly-1PM/shelly1pm.status.ram_total)*0.9`|Warning|<p>-</p>|
|Shelly 1PM: Memory usage >=90%|<p>-</p>|`last(/Shelly-1PM/shelly1pm.status.ram_free)>=last(/Shelly-1PM/shelly1pm.status.ram_total)*0.9`|Average|<p>-</p>|

## Feedback

Please report any issues with the template at the official Zabbix community template repository.

## Version History

### 7.0
- Migrated template to Zabbix 7.0 format
- Updated version field to '7.0'
- Added "Shelly 1PM:" prefix to all trigger names for better identification
- Updated export date to 2024-08-26
- All UUIDs preserved for backward compatibility
- Template functionality remains identical to 6.0 version

### 6.0
- Initial version by Leonard Winck
- Comprehensive monitoring of Shelly 1PM device via HTTP API
- Power consumption monitoring with dependent items
- Network connectivity monitoring (WiFi, Cloud, MQTT)
- Temperature and system health monitoring
- Relay state monitoring and control feedback