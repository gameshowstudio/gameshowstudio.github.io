---
layout: page
title: Press Kit
permalink: /press/
nav_menu_title: Press Kit
redirect_from: "/home/press"
---

Thanks for your interest in Game Show Studio! This Press Kit gives additional information and resources that are not listed on the [home page](/). If you would like additional information, please feel free to contact the developer at [tim@gameshowstudioapp.com](mailto:tim@gameshowstudioapp.com).

## Resources

* [Demonstration Video](https://youtu.be/8EqQc93Jzaw){:target="_blank<!-- markup clean_ -->"} (1 minute, also embedded below)
* [Game Show Studio Help Pages](/help)
* Logo and Icon
    * [App Icon (1024 x 1024)](/images/press/gssIconRound1024.png){:target="_blank<!-- markup clean_ -->"}
    * [Logo (1024 x 312)](/images/press/logoWithText1024x312.jpg){:target="_blank<!-- markup clean_ -->"}
* Images
    * Image of Multiple Devices Connected During Game in Progress
        * [iPad](/images/press/host-and-players-pad.png){:target="_blank<!-- markup clean_ -->"}
        * [iPhone](/images/press/host-and-players-phone.png){:target="_blank<!-- markup clean_ -->"}
    * Image of Host Connected to Apple TV
        * [iPad](/images/press/host-and-tv-pad.png){:target="_blank<!-- markup clean_ -->"}
        * [iPhone](/images/press/host-and-tv-phone.png){:target="_blank<!-- markup clean_ -->"}
* [App Update History](/updates)
* [App Store Download Page](https://itunes.apple.com/us/app/game-show-studio/id924249807?ls=1&mt=8){:target="_blank<!-- markup clean_ -->"}

{% include youtube-player.html id="8EqQc93Jzaw" %}

## Standout Features

### Multiple Players per Device

Up to four players can play on each device that connects to a host’s device. This makes playing with many people easy, even in groups that include people who do not have an iOS device.

![image of host and players](/images/press/host-and-players-pad-w1200.png)

### Customizable Teams

The host can configure teams in many different ways, including teams without equal numbers of players. Teams are not tied to which players may be sharing a device; two players can buzz in from the same device, but be on different teams.

### Customizable Rules Make for an Easy-to-Run Game

{: .floatRight .smallerImageOnPhone}
![host's round rules screen](/images/press/round-configuration.png){:width="280px"}

The host has control over scoring and timing rules. Different sets of rules can be prepared before the game begins so that the host can easily put on a game that's played with various rounds, each with different timing and scoring rules.

Because there is always a set of active round rules, when a player buzzes in, the only action necessary from the host is to tap whether the player answered correctly or incorrectly. The score will automatically be updated based on the host’s choice, meaning that the host can concentrate on running an exciting game without worrying about the math. The host also has the option to clear the buzzers without adjusting the score to quickly remedy inadvertent taps from overzealous players.

It is quick and easy to make scoring corrections any time during the game by tapping on any team's score. A host can quickly type in any score, or use the Quick Update buttons, which adjust the team's score based on the current round's "Points for Correct" and "Points for Incorrect" values.

![scoring correction screen](/images/press/scoring-correction.png){:width="220px"}

*A portion of the screen that allows scoring corrections to be made when the Points for Correct is set to ten and Points for Incorrect is set to five. Note the Edit Score button, which allows for free-form score editing, as well.*

For more information, check out the [Round Rules page](/help/roundrules).

### Music and Sound Effects

Sounds play automatically throughout the game, so that the host can easily create an immersive game show feel. Sounds are played automatically when:

* a player buzzes in,
* a player answers a question correctly,
* a player answers a question incorrectly,
* timers run out.

The volume of these sounds can be adjusted on a per-effect basis in the Sound Pane, as shown here:

![sound pane](/images/press/sound-effect-mixers.png){:width="300px"}

There are also sounds and music that play automatically during the [Timed Round](/help/timedround).

For more information about music that's available to be played in the app, check out the [Music page](/help/music). Music is also played when certain screens are displayed on the TV, as described on the [TV page](/help/tv). Sets of round rules also have music associated with them, as described on the [Round Rules page](/help/roundrules).

All of the music and sound effects in the app were created by the developer and his brother. These tracks help to provide an immersive game show feeling while playing.

### TV Integration

Game Show Studio is designed to work with or without a TV, which, when connected, displays scores and timers, adding to the “Studio” feel. When connected to a TV, sound effects and music are routed to the TV. All of the necessary information to host a game is displayed on the host’s screen, making the additional display optional.

Check out the [TV page](/help/tv) for more information.

![image of host connected to a TV](/images/press/host-and-tv-pad-w1200.png)

## Use Cases

Game Show Studio is great for a variety of environments, including:

* House Parties: Take existing trivia board games to the next level by adding buzzers next time you play.
* Bridal/Baby Showers: Prepare questions about the couple or expecting parents, combined with fun general wedding/baby questions, for what will surely be a memorable experience.
* Holiday Parties: We have used Game Show Studio for New Year's Trivia, where we wrote questions about the year that just passed (e.g. top movies, top 10 Google searches) and about New Year's traditions. A host can prepare themed questions for any holiday.
* Classrooms: Teachers can engage their students in a whole new way with Game Show Studio. One App Store review that we are proud of reads, “I'm a high school teacher at a school where students use iPad, and teachers have iPad and Apple TV, and this app is INCREDIBLE. Revolutionizes the review game. The kids love it. I love it. It's so fun. If you're a teacher that's connected with apple products, you must have this app.” Our developer is a former teacher, and he loves knowing that he is helping other teachers with this app.
* Business: Game Show Studio can make your meetings and presentations more interactive and engaging, and is great for team building activities.

Game Show Studio uses mobile devices to bring people together in a meaningful way, interacting with one other in ways that go beyond what the device itself can facilitate. The interaction style is a lot like a board game that is played with people in the same room, and we think that makes this app special. Game Show Studio provides a great way to get friends, family, students, and colleagues talking and laughing together in friendly competition.

## Continued Development

Game Show Studio has enjoyed numerous [updates](/updates) during its lifetime, with new features that give hosts an increasing number of exciting ways to put on a game show.

#### Version 1 Updates
* Version 1.0: January 30, 2015
* Version 1.1: February 18, 2015 - Buzzer timing enhancement.
* Version 1.2: March 12, 2015 - Ability to customize which sounds play during the game.
* Version 1.3: April 6, 2015 - More reliable networking mode (see [Networking Details](#networking-details) below for details).
* Version 1.4: May 10, 2015 - New song collection (Intrigue) and new ambient track (Suspension).

#### Version 2 Updates

{% assign pages = site.pages | where: "layout", "update" | sort: "updateversion" %}
{% for page in pages %}
{%- assign majorversion = page.updateversion | split: "." | first -%}
{%- if majorversion == "2" -%}
* [Version {{page.updateversion}}]({{page.permalink}}) · {{page.releasedate}}: {{page.updatesummary}}
{% endif %}
{%- endfor -%}

<br>

#### Version 3 Updates

{% for page in pages %}
{%- assign majorversion = page.updateversion | split: "." | first -%}
{%- if majorversion == "3" -%}
* [Version {{page.updateversion}}]({{page.permalink}}) · {{page.releasedate}}: {{page.updatesummary}}
{% endif %}
{%- endfor -%}

<br>

## System Requirements

Game Show Studio is designed for iPhone and iPad and supports devices running iOS 12 and above. Devices running older versions of iOS with a previous version of the app installed are still able to host and join games including devices running the current version of Game Show Studio.

## Networking Details

Game Show Studio provides the option to choose between two networking modes, so that the host can provide the best experience based on the devices that are participating. The more reliable networking mode is not supported by older devices (such as iPad 2), so Compatibility Mode is offered to allow a host to facilitate a game with such devices. Check out the [Finding Players page](/help/findingplayers) for more details about

* fixing connection problems,
* the networking modes, and
* the number of devices that can join a game.

For more technical information about how wireless connections work on Game Show Studio, check out our [Networking Details page](/press/networkingdetails).

## Pricing

Downloading Game Show Studio is free. Joining a game as a player is free. A $7.99 (US) In-App Purchase is required to host a full game. This pricing model was selected because we wanted to make it easy for a host to get a lot of people interested in playing a game (it is a low barrier to ask people to download a free app). This follows the spirit of a board game, where only one person needs to make the purchase for many people to enjoy it. We hope that users will compare the cost and value of this app to that of a board game.

### Free Host Mode Upgrades from Any Previous Version to Version 3

Customers who purchased Hosting Mode in either version 1 or version 2 will get a free upgrade to Hosting Mode in version 3.

### Hosting Trial

Users have the opportunity to experience a hosting trial as part of the free app download. All hosting functionality is available during this trial, including:

* connecting to players,
* assigning players to teams,
* playing music and sound effects, and
* connecting to a TV.

The only feature that is not available during the trial is the ability to purchase additional question sets. The trial ends after players buzz in twice. The trial mode can be used an unlimited number of times; each time it is used, the game ends after players buzz in twice. The In-App Purchase unlocks the ability to host games with no buzz-in limit an unlimited number of times.

To enter the Hosting Trial, select the "Host" option from the first screen in the app.

### Question Sets

Game Show Studio comes with a collection of question sets available for free. The free sets are designed to form the basis of a game with several rounds of play. Additional question set collections are available as an In-App Purchase.

## Responsive Host Screen

A lot of thoughtful consideration went into finding the best way to give the host clear access to the most important controls while they host a game. On larger displays, more controls are available the host's screen at any given time. On smaller displays (such as on a phone), controls are grouped and are quickly accessible by changing which control pane is visible through one tap on a segmented control.

## Player Screen - Optimized for Buzzing In

The goal for the players’ buzz in screen was to provide the biggest possible touch area for buzzers while still providing the players with options to leave the game or change their names. This meant that the configuration of the screen did not need to change with the device size; any device, regardless of size, will be filled with one or more buttons to tap to buzz in.

The configuration does change slightly, though, based on how many players are using the device. If there are only one or two players on the device, the option buttons appear at the top of the screen. With three or four players, though, it’s probable that players would be gathered around the device, meaning that allowing the players to tap all the way to any edge (including the top) to buzz in would be ideal. In that case, the option buttons are located in the center of the screen, at the intersection of all of the buttons, where players would be unlikely to tap. This provides a great experience for players regardless of how many people are sharing a device.

![buzz in screen examples with one through four players](/images/press/players-1-2-3-4.png)
