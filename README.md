# Bruno-Robot

**⚠️ Note:** This is a working document that will certainly be changed a lot :)

[![Discord](https://img.shields.io/discord/971137288471998574?logo=discord)](https://discord.gg/nBFmWqZT9V)
[![Check Links](https://github.com/bruno-robot/bruno-robot/actions/workflows/check-links.yml/badge.svg)](https://github.com/bruno-robot/bruno-robot/actions/workflows/check-links.yml)

TLDR: Starting out with soccer playing robots is too complicated.

## Motivation

Let's start with the objective of the RoboCup:

> By the middle of the 21st century, a team of fully autonomous humanoid robot soccer players shall win a soccer game, complying with the official rules of FIFA, against the winner of the most recent World Cup.

*Source: [robocup.org](https://www.robocup.org/objective)*

To achieve this ambitious goal in the remaining 28 years, the rules are tightened every year to bring them in line with those of FIFA.
In addition, it's essential to motivate young researchers to participate, which is why schoolchildren are already encouraged to develop robots for RoboCupJunior.
After more than 20 years of RoboCupJunior though, the needed technologies/electronics have reached a level that makes it increasingly more difficult for newcomers to enter the competition.
This is why some regions (i.e. germany) have decided to introduce specific entry leagues, restricting allowed parts dramatically in order to reduce cost and complexity (most commonly LEGO + Fischertechnik only).
Recently though, Lego has retired the MINDSTORMS EV3 and related components (*Source: [legoeducation.com](https://community.legoeducation.com/blogs/36/95)*).
Additionally, the successor to LEGO Mindstorms - Robot Inventor - provides neither IR nor camera sensors, which are however indispensable for participation.
The reason for this is that the new Robot Inventor app does not yet offer the option of integrating non-official sensor blocks.
It's unclear whether LEGO will ever change this, posing a potential threat to the ease of entry for new and established teams alike.

## Our Proposal

Notes:

* We want a platform to make getting into the RoboCupJunior Soccer competition easier and (potentially much) more affordable.
* This project should be sustainable and not depend on company interests/decisions
  * Therefore open source / open hardware

## What we DO NOT want

* a ready-to-play robot
  * TODO: explain deeper
  * Too weak of a software framework for teams to reasonably get started
  * No full tutorial on "how to play soccer"
  * Just extensible electronics/hardware(adapter) kits. Soldering/mounting still required.
* S perfect system which outperforms current world champions
  * Similiarily to LEGO robots, Bruno should be capable of attending any current league but not straight up outperform other robots without *significant* improvements made by individual teams.
  * TODO: explain deeper

## Schedule

1. Developing basic components, test it with select teams in lightweight / open league
2. Let teams gather experience on early designs and incorporate their feedback back into the project.
3. Convince the german committee for admission in the standard league

## Who we are

We are a group of former participants, coaches, referees, volunteers of RoboCupJunior Soccer.
We are not a company and have no commercial interest.
However, we are thinking about founding a non-profit organization at some point in order to be able to distribute the robot parts developed here as kits without unnecessary price markups, while potentially increasing part availability in the process and thereby improving sustainability.

## Call for Contribution

do this is in "our proposal"?

## Notes

* NO commercial goals at all
* Beginner friendliness as there is a big step between Lego and own electronics already today
* Big teams have it anyways
* Everything is open source technical and communication -> everybody can contribute
* Project does NOT provide play-ready software, only libraries
* Project provides only plans/layout for electronics and omniwheels
* See all our design on our [decision board](decision-board.md)

## TODO

* [ ] check (R) on all Logos
* [ ] check spelling of LEGO, fischetechnik, Robocup
* [ ] TLDR
