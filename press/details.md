---
layout: page
title: Sweating the Details
permalink: /press/details/
---

We’re proud of this app, and we put a lot of thought into the experience. This page points out a few small details that add an extra bit of polish to Game Show Studio.

## App Launch Animation

The app was designed so that the icon and initial screen have the same elements in the same location. This makes for a fluid experience when the user launches the app from the iOS home screen, and the app icon zooms to fill the screen (the default launch animation in iOS 7, 8, and 9).

## Responsive Host Screen

A lot of thoughtful consideration went into finding the best way to give the host clear access to the most important controls while they host a game. Naturally, the best solution was different depending on device size. Here are some ways that responsive design was used to provide a great hosting experience, regardless of the size of device:

* *Assigning players.* Hosting on iPad offers an intuitive drag-and-drop interface for assigning players to teams, taking advantage of the screen space to make all players visible at all times. On iPhone, the limited screen space meant that a context switch was better for team assignments. As part of the iPhone connection flow, after browsing for players, the Assign Players screen is automatically displayed if there is at least one connected device. The Assign Players screen can also be accessed directly from the Game Options menu.
* *A/V, Round Rules, and Questions Panes.* On iPad, two extra panels (in addition to the Teams Panel) are visible at all times. One of them is the A/V panel, which can switch between the Music Pane, the Sound Pane, and the TV Pane. The other panel contains the Questions Pane and the Round Rules Pane. All of these panes are available on iPhone, as well, but because of the smaller screen space, only one pane can be onscreen at a time.
* *The score/buzz in display.* On iPad, the teams and scores are always visible on the main host screen. On iPhone, other panes (like the Music Pane or the Questions Pane) take the place of the Teams Pane when they are visible. To make sure that the host always has access to relevant information, an informational view appears in order to show the current scores whenever there are players on teams and the Teams Pane is not visible. When a player buzzes in, this informational panel animates to show which player buzzed in. This way, the host can stay on a pane other than the Teams Pane (such as the Questions Pane) throughout the entire game. This informational view is pictured below, where you can see what it looks like in its default state, and in the state where a player has buzzed in.
<br>
![score info pane](/images/v2-0-0/score-and-buzz-in-info-pane-both.png){:width="440px"}
<br><br>
* *Other smaller details.* There are additional items that behave slightly differently so that the screen space is used in an optimal way. On iPad, the New Game button is on the main host screen, but it's in the Game Options menu on iPhone. Writing custom questions works slightly differently across the devices. We took care to create a great experience, both in big ways, and for small details.

## Player Screen

The goal for the players’ buzz in screen was to provide the biggest possible touch area for buzzers while still providing the players with options to leave the game or change their names. This meant that the configuration of the screen did not need to change with the device size; whatever size the user has will be filled with one or more buttons.

The configuration does change slightly, though, based on how many players are using the device. If there are only one or two players on the device, the option buttons appear at the top of the screen. With three or four players, though, it’s probable that players would be gathered around the device, meaning that allowing the players to tap all the way to any edge (including the top) to buzz in would be ideal. In that case, the option buttons are located in the center of the screen, at the intersection of all of the buttons, where players would be unlikely to tap. This provides a great experience for players regardless of how many people are sharing a device.

![buzz in screen examples with one through four players](/images/v2-0-0/buzz-in-responsive.png)
