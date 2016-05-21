---
layout: page
title: Press Kit
permalink: /press/
nav_menu_title: Press Kit
---

Thanks for your interest in Game Show Studio! This Press Kit gives additional information and resources that are not listed on the [home page](/). (Please start by reviewing the main features of the app on the [home page](/) if you haven't already.) If you would like additional information, please feel free to contact me at [tim@gameshowstudioapp.com](tim@gameshowstudioapp.com).

## Resources

* [Demonstration Video](https://youtu.be/0eBBkWw2kg0) (1 minute, also embedded below)
* [App Icon (1024 x 1024)](/images/gssIconRound1024.png)
* [Logo (1024 x 312)](/images/press/logoWithText1024x312.jpg)
* [Image of multiple devices connected during game in progress](/images/press/hostAndPlayers2208.png)
* [Image of host connected to Apple TV](/images/press/hostAndTV1669.png)
* [App Store Download Page](https://itunes.apple.com/us/app/game-show-studio/id924249807?ls=1&mt=8)

{% include youtube-player.html id="0eBBkWw2kg0" %}

## Standout Features

### Multiple Players per Device

Up to four players can play on each device that connects to a host’s device. This makes playing with many people easy, even in groups that include people who do not have an iOS device.

![image of host and players](/images/hostandplayers800.png)

### Customizable Teams

The host can configure teams in many different ways, including teams without equal numbers of players. Teams are not tied to which players may be sharing a device; two players could be buzzing in from the same device, but be on different teams.

![teams example](/images/press/teams2221.png){:width="360px"}
![teams example](/images/press/teams211111.png){:width="360px"}

![teams example](/images/press/teams2311.png){:width="360px"}
![teams example](/images/press/teams111111.png){:width="360px"}

![teams example](/images/press/teams61.png){:width="360px"}
![teams example](/images/press/teams1010.png){:width="360px"}


### Customizable Rules Make for an Easy-to-Run Game

{: .floatRight .smallerImageOnPhone}
![host's round rules screen](/images/press/hostRoundRules.png){:width="280px"}

The host has control over scoring and timing rules, so that when a player buzzes in, the only response necessary from the host is to tap whether the player answered correctly or incorrectly. The score will automatically be calculated based on the host’s choice, meaning that the host can concentrate on running an exciting game and not worry about the math. Clearing the buzzers without adjusting the score is also possible to quickly remedy inadvertent taps from overzealous players.

Sounds play automatically anytime a player buzzes in, answers correctly, or answers incorrectly. Sounds also play when timers run out. Any of these sounds can be turned off in the Round Options screen. (To access Round Options, tap the black rounded rectangle with the round information on iPad. On iPhone, tap “Game Options” then tap “Round Options.”)

It is possible to make score corrections any time during the game. To do so on iPad, tap the team header that shows the score. On iPhone, tap anywhere on the cell that lists the team members and the score.

### Music and Sound Effects

All of the music and sound effects in the app were created by [my brother and me](/about). These tracks help to provide the Game Show feeling while playing.

### Apple TV Integration

Game Show Studio is designed to integrate with an Apple TV which displays scores and a timer, adding to the “Studio” feel. When connected to an Apple TV, sound effects and music are routed to the TV. Game Show Studio works great with or without an Apple TV. All of the necessary information to host a game is displayed on the host’s screen, making the additional display optional.

To connect to an Apple TV, swipe up from the bottom of the screen to display Control Center. If an Apple TV is nearby, tap the AirPlay button. Tap the Apple TV you would like to connect to and make sure that Mirroring is on.

![image of host connected to a TV](/images/hostandtv800.png)

## Sweating the Details

I’m proud of this app, and I put a lot of thought into the experience. There are a few minor details that illustrate this that I would like to point out if you are interested. Check them out [here](/press/details).

## Use Cases

Game Show Studio is great for a variety of environments, including:

* House Parties: Take existing trivia board games to the next level by adding buzzers next time you play.
* Bridal/Baby Showers: Prepare questions about the bride or expecting parents, combined with fun general wedding/baby questions, for what will surely be a memorable experience.
* Holiday Parties: I have used Game Show Studio for New Year's Trivia, where I wrote questions about the year that just passed (e.g. top movies, top 10 Google searches) and about New Year's traditions. Similar things could be done for any holiday.
* Classrooms: Teachers can engage their students in a whole new way with Game Show Studio. At the time of this writing, the review on the App Store that has made me feel the best reads, “I'm a high school teacher at a school where students use iPad, and teachers have iPad and Apple TV, and this app is INCREDIBLE. Revolutionizes the review game. The kids love it. I love it. It's so fun. If you're a teacher that's connected with apple products, you must have this app.” As a former teacher, I love knowing that I am helping other teachers.
* Business: Game Show Studio enables more interactivity during meetings or presentations.

Game Show Studio uses mobile devices to bring people together in a meaningful way, interacting with one other in ways that go beyond what the device itself can facilitate. The interaction style is a lot like a board game that is played with people in the same room, and I think that makes this app quite special. Game Show Studio provides a great way to get friends, family, students, and colleagues talking and laughing together in friendly competition.

## Continued Development

Game Show Studio has enjoyed frequent updates since its initial release, with new user-facing features:

* Version 1.0: January 30, 2015
* Version 1.1: February 18, 2015 - Buzzer timing enhancement.
* Version 1.2: March 12, 2015 - Ability to customize which sounds play during the game.
* Version 1.3: April 6, 2015 - More reliable networking mode (see Networking Details below for details). This was the feature I was waiting to ship before considering Game Show Studio ready to be marketed.
* Version 1.4 - May 10, 2015 - New song collection (Intrigue) and new ambient track (Suspension).

## System Requirements

Game Show Studio is designed for iPhone and iPad. It supports iOS 7 and above and is optimized for iPhone 5, iPhone 6, and iPhone 6 Plus.

## Networking Details

Game Show Studio was initially implemented using Apple's Multipeer Connectivity framework, which connects devices using “infrastructure Wi-Fi networks, peer-to-peer Wi-Fi, and Bluetooth personal area networks.” In testing, this framework seemed to reliably support only up to four devices connected to a host. This was the only networking option available in versions 1.0 through 1.2.

Due to the limited number of connections available using Multipeer Connectivity, in addition to concerns I had about reliability, I developed an implementation using Core Bluetooth, which connects devices using Bluetooth Low Energy (BLE). This new implementation's connections were more reliable, even with more devices. The drawback is that older iOS devices (including iPad 2, popular with education users) do not support BLE, and if I removed Multipeer Connectivity, I would suddenly have left users behind who may have just started using this new app.

I decided to ship version 1.3 with both networking modes. The biggest user-facing drawback to this was the added complication. I tried to minimize this impact by simplifying the process as much as possible, to the point that it is transparent to players (only the host has to choose a networking mode). When a player begins scanning for a host, both networking modes are invoked (if supported) so that the host will find the device regardless of which mode the host's device is in. If a player's device does not support BLE, the user is informed that the host will need to be in non-BLE mode to be discovered.

The only user who has to make a choice of networking mode is the host.  The default mode is the more reliable mode, BLE (if supported). Brief explanations of the advantages of each mode are provided to the host, so that if an older, non-BLE device is involved, the host can easily switch to the mode that supports it.

## Number of Devices

As I mentioned above, using non-BLE mode, a host can reliably connect to up to four player devices.

During a test of all the BLE devices I could get my hands on, I was able to reliably connect to all of them (five player devices). I think that the number that would work is higher than that, but since I was unable to test it due to the number of devices I had access to, the game officially supports up to five player devices connected to a host in BLE mode. If the host attempts to connect to more devices, the user will be informed that doing so is not tested, but can choose to proceed with the connection attempts. I hope for an opportunity to test with more devices soon.

Each player device can support up to 4 players, so in BLE mode, up to 20 players are officially supported (although it is likely that more could join in practice).

## Pricing

Downloading Game Show Studio is free. Joining a game as a player is free. A $7.99 In-App Purchase is required to host a full game. This pricing model was selected because I wanted to make it easy for a host to get a lot of people interested in playing a game (it is a low barrier to ask people to download a free app). This follows the spirit of a board game, where only one person needs to make the purchase for many people to enjoy it. I hope that users will compare the cost and value of this app to that of a board game.

## About the Developer

Check out the [About Us](/about) page for more information.
