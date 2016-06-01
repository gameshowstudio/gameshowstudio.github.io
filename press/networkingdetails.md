---
layout: page
title: Networking Details
permalink: /press/networkingdetails/
---


Game Show Studio was initially implemented using Apple's [Multipeer Connectivity framework](https://developer.apple.com/library/ios/documentation/MultipeerConnectivity/Reference/MultipeerConnectivityFramework/index.html){:target="_blank<!-- markup clean_ -->"}, which connects devices using “infrastructure Wi-Fi networks, peer-to-peer Wi-Fi, and Bluetooth personal area networks.” In testing, this framework seemed to reliably support only up to four devices connected to a host. This was the only networking option available in versions 1.0 through 1.2.

Due to the limited number of connections available using Multipeer Connectivity, in addition to concerns we had about reliability, we developed an implementation using [Core Bluetooth](https://developer.apple.com/library/ios/documentation/NetworkingInternetWeb/Conceptual/CoreBluetooth_concepts/AboutCoreBluetooth/Introduction.html){:target="_blank<!-- markup clean_ -->"}, which connects devices using Bluetooth Low Energy (BLE). This new implementation's connections were more reliable, even with more devices. The drawback is that older iOS devices (including iPad 2) do not support BLE, and if we removed Multipeer Connectivity, we would have suddenly left users behind who may have just started using this new app.

We decided to ship version 1.3 with both networking modes. The biggest user-facing drawback to this was the added complexity. We tried to minimize this impact by simplifying the process as much as possible, to the point that it is transparent to players (only the host has to choose a networking mode). When a player begins scanning for a host, both networking modes are invoked (if supported) so that the host will find the device regardless of which mode the host's device is in. If a player's device does not support BLE, the user is informed that the host will need to be in non-BLE mode to be discovered.

The only user who has to make a choice of networking mode is the host. The default mode is the more reliable mode, BLE (if supported). Brief explanations of the advantages of each mode are provided to the host, so that if an older, non-BLE device is involved, the host can easily switch to the mode that supports it. In version 2.0, the messaging on the host's screen was simplified even further:

* When Reliable Mode is selected (the default case), the host now sees a "Don't See Who You're Looking For?" button on the Find Players screen.
* When Compatibility Mode is selected, the host sees a "Switch Back to Reliable Mode" button on the Find Players screen.

Regardless of which button is visible, tapping the button will display a message with information about changing networking modes, with options to confirm the change or cancel the change.

## Networking on iPad Pro 9.7"

Tests using the iPad Pro 9.7" as the host have shown that the device will not maintain a connection to more than three player devices while in Reliable Mode. Attempts to connect to more than three devices fail. Other newer devices (like the iPhone 6s) allow connections to many more than three devices. We suspect that this is due to a hardware change in the iPad Pro 9.7", and we are continuing to investigate this issue.

For more information, check out our [Finding Players page](/help/findingplayers).
