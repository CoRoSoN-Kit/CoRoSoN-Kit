# CoRoSoN-Kit

**Co**mponents for **Ro**bocupJunior **So**ccer **N**ewcomers

[![Discord](https://img.shields.io/discord/971137288471998574?logo=discord)](https://discord.gg/xTAptqNB7J)
[![GitHub Mega-Linter](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/workflows/Lint%20Code%20Base/badge.svg)](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/actions/workflows/linter.yml)
[![License](https://img.shields.io/github/license/CoRoSoN-Kit/CoRoSoN-Kit)](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/blob/main/LICENSE)

## TLDR

- Starting out with RoboCupJunior Soccer is complicated.
- LEGO®[^lego] MINDSTORMS®[^lego] is retired.
- Let's develop components helping RoboCupJunior newcomers participate.

_Note: We only give instructions for components here, which have to be built by teams themselves. So it is not as easy as using LEGO®[^lego] MINDSTORMS®[^lego]._

## Motivation

Let's start with the objective of the RoboCup:

> By the middle of the 21st century, a team of fully autonomous humanoid robot soccer players shall win a soccer game, complying with the official rules of FIFA, against the winner of the most recent World Cup.

_Source: [robocup.org](https://www.robocup.org/objective)_

To achieve this ambitious goal in the remaining 28 years, the rules are tightened every year to bring them in line with those of FIFA.
In addition, it's essential to motivate young researchers to participate, which is why schoolchildren are already encouraged to develop robots for RoboCupJunior.

After more than 20 years of RoboCupJunior though, the needed technologies/electronics have reached a level that makes it increasingly more difficult for newcomers to enter the competition.
This is why some regions (i.e. germany) have decided to introduce specific entry leagues, restricting allowed parts dramatically in order to reduce cost and complexity (most commonly LEGO®[^lego] + Fischertechnik only).
Recently though, LEGO®[^lego] has retired the MINDSTORMS®[^lego] EV3 and related components (_Source: [legoeducation.com](https://community.legoeducation.com/blogs/36/95)_).

Additionally, the LEGO®[^lego] MINDSTORMS®[^lego] successor to the EV3 - Robot Inventor - provides neither IR nor camera sensors, which are however indispensable for participation.
The reason for this is that the new Robot Inventor app does not yet offer the option of integrating non-official sensor blocks.
It's unclear whether LEGO®[^lego] will ever change this, posing a potential threat to the ease of entry for new and established teams alike.

## Our Proposal

We want a platform to make getting into the RoboCupJunior Soccer competition easier and (potentially much) more affordable.
Perhaps even filling part of the gap that LEGO®[^lego] may create in the near future.
This project should be sustainable and not depend on any company interests or decisions.
We want to develop basic components which Teams can build and improve by themselves.

Any development will be open source and open hardware.
The try to make the process as transparent as possible.
Any discussions will be public (here and/or discord) such that everyone is able to understand why we have decided for or against certain things.

We would love to see robots build with the CoRoSoN-Kit in the standard leagues where LEGO®[^lego] robots are allowed today.
Until then, the components can be used in the LightWeight and Open League.

### Components

Currently monitored components of the CoRoSoN-Kit.

| Component                      | Status                                                                                                                          |
|--------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
| Brain/Main CPU                 | [🧠 #18](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/18) & [🧠 #44](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/44) |
| User Interface                 | [🧠 #23](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/23)                                                                  |
| Orientation sensor             | [🧠 #22](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/22)                                                                  |
| Line detection                 | [🧠 #24](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/24)                                                                  |
| IR detection module            | [🧠 #25](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/25)                                                                  |
| Motor + driver                 | [🧠 #2](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/2)                                                                    |
| Omniwheel                      | [🧠 #26](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/26)                                                                  |
| IDE integration                | [🧠 #27](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/27)                                                                  |
| Visual-Programming integration | [🧠 #28](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/28)                                                                  |
| Kicker                         | ❓                                                                                                                               |
| Dribbler                       | ❓                                                                                                                               |
| Camera                         | [❓ #34](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/34)                                                                   |

Legend:

<!-- * 📋: Planned -->

- ❓: In Discussion (Should we ever do that?)
- 🧠: Brainstorming ongoing (Issue linked)
- 🚧: In active development
- ✅: Done
- ❌: Not planned

See all of our current design decicions on our [decision board](decision-board.md).

## What we DO NOT want

To allow RoboCupJunior teams to use our components, the [RCJ Soccer rules](https://junior.robocup.org/wp-content/uploads/2022Rules/2022_Soccer_Rules_final01.pdf) must be abided by. In particular:

> Robots must be constructed and programmed exclusively by student members of the team. Mentors,
> teachers, parents or companies should not be involved in the design, construction, assembly, programming or debugging of robots.

_Source: §Preface_

In order not to violate these rules:

- We **DO NOT** offer a ready-to-play robot.
  - Instead, we offer a set of instructions to build components.
  - Production of the components (soldering / mounting / 3D-Printing / etc.) and
  - assembling the components (creating base plates, developing a chassis, etc.) still needs to be done by the teams.
- We **DO NOT** offer a software which plays soccer.
  - Instead, we are only providing libraries to use our components.
- We **DO NOT** want to give any one team an advantage.
  - Let our transparency and open accessibility for everyone serve as proof of this.
- We **DO NOT** provide a tutorial on _"how to play soccer"_ (or similar)
  - Teams must develop _all_ strategies / higher-level logic / etc. to play soccer themselves.
- We **DO NOT** want a _highly_ competitive system which outperforms others out of-the-box
  - We will not to provide the fastest motors, the best camera, the most powerful processors, etc. Instead we provide basic components which are affordable and available to everybody.
  - To actually win tournaments, individual teams would need to _substantially_ change and improve all components.

To summarize: Similar to LEGO®[^lego] robots, the CoRoSoN-Kit should be composable into a robot capable of attending any current league with relative ease, but it will always require a significant effort by the individual teams themselves.

## Who we are

We are a group of former participants, coaches, referees, volunteers of RoboCupJunior Soccer.
We are not a company and have no commercial interest.
However, we are thinking about founding a non-profit organization at some point.
For example, this would give us the opportunity to distribute circuit board blanks (to be assembled) or electronic parts as sets without unnecessary price markups.

### Call for Contribution

The CoRoSoN-Kit is open-source for a reason and that is you.
If you are passionate about the robocup and its goals
our team is not fixed and we are always open to _your_ contribution.
Whether development, discussion, questions, feedback or criticism:
Everything is welcome!

Especially to teams utilizing the CoRoSoN-Kit: You are very welcome to play back your improvements, find the bugs we made in the libraries or just send us pictures of your robot. This way we can all celebrate the success of the robots in 2050 🤖⚽🏆.

### Contributing

If you want to contribute to the CoRoSoN-Kit, please read our [contribution guidelines](.github/CONTRIBUTING.md).

[^lego]: Disclaimer: LEGO® and MINDSTORMS® are trademarks of the LEGO® Group, which does not sponsor, authorize or endorse this site.
