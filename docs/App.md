# mySunPower app

## Home tab - Live Data

This tab shows power flow between the grid, your home, your panels, and your battery (if installed).

It will display the "last received" data time if the data is over 5 minutes out-of-date.

The tab is populated from the monitoring backend via MQTT.

## SunVault tab (some systems) - Battery Settings

This tab allows setting the discharge controller mode (Reserve, Self-Supply, or Cost Savings) and how much battery capacity is "held back" for power outages.

The Cost Savings mode is not fully functional since late 2024.  The rate picker and server-side tariff data ceased working.

As a result, Cost Savings mode will fall back to its default of discharging 4-8pm on weeknights.  This cannot be timing cannot be configured through the app.

## Analyze tab - Historical Data

This tab shows historical data.  It can be incorrect for various reasons.

## Panels tab (some systems) - Microinverter data

This tab is only available if your installer produced a panel map and enabled the tab for you while SunPower was around.

## Profile

The "System Connection" section is frequently wrong.  For example, it will show "System is communicating via Ethernet" when it's on Wi-Fi, and vice-versa.

### SunVault Info

You can "Reset Battery" from here.  This will only work if your PVS is communicating with the monitoring servers.
