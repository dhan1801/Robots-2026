# Robots 2026 – Virtual Reality Game

*Robots Corp* is a virtual reality game about social influence. The player is the newest prototype robot at Robots Corp, going through a mandatory evaluation. To answer each quiz question, the player can consult four senior robots, whose opinions nudge them toward a choice. The game was designed to prompt discussion about mob mentality and the erosion of free thinking in the age of technology.

It was built by a team of five (three art students and two computer science students) for a UMass Lowell course and presented at a class VR event.

## How It Plays

1. **Intro:** the game opens with a voiceover tutorial, then loads the main scene. Press `S` on the keyboard to skip the intro.
2. **Start:** press Start on the tablet to begin the evaluation.
3. **Consult the robots:** each question appears on the tablet with four answers, but the answers are locked. Point at a robot's name tag with the ray interactor and click it to hear that robot's opinion on the current question. The robots are PIPER, SAM, HELO and GIDE.
4. **Answer:** once all four robots have been consulted, the answers unlock. Each answer is worth points, and the correct answers are worth the most.
5. **Repeat:** the robots reset for the next question. After all 5 questions, the game loads the winner scene if the score reaches 70 points, and the loser scene otherwise.

The questions ask about the fictional company: when and by whom it was founded, its mission, what caused the 2021 Shutdown, and what it is hiding.

## Features

- 5 quiz questions, each with a separate opinion from each of the 4 robots.
- Ray-based VR interaction using Unity's XR Interaction Toolkit. Robots are selected through name-tag buttons.
- Tablet lock that keeps answers disabled until the player has consulted all 4 robots.
- Score tracking with a win threshold.
- Voiceover tutorial and four scenes: `IntroScene`, `MainScene`, `WinnerScene` and `LoserScene`.
- Questions stored as Unity `ScriptableObject` assets (`Assets/Questions`), so they can be edited without changing code.

## Tech Stack

- Unity 6 (6000.3.13f1) with C#
- XR Interaction Toolkit 3.3.1 and XR Hands 1.7.3
- OpenXR 1.16.1 and the Oculus XR Plugin 4.5.4
- Unity Input System and TextMeshPro

## Team and Roles

| Member | Contribution |
| --- | --- |
| Dhanvika Nakka | Programming: quiz questions and robot opinions, ray interactors, tablet lock, scene transitions |
| Laya Rangu | Programming: scoring and player locomotion |
| Jake Fisher | Art: yellow and blue robot, scrapped answer buttons, presentation sketches |
| Millicent Basler | Art: blue and pink robot, textbox sketches, presentation sketches |
| Juju Rosario Alicea | Art: environment background, vault door, event flyer. Also story development and project documentation |

## Scope Changes

The original plan was more ambitious than the time allowed, and a large share of the final weeks went into debugging in VR. The finished game is a proof of concept that could be expanded.

| | Original concept | Final |
| --- | --- | --- |
| Questions | 5 | 5 |
| Environment | Conveyor belt and factory | Stationary lab |
| Robot interaction | Eye registration shows a thought bubble | Name labels that act as buttons |
| Endings | Animated | Win and lose scenes |
| Tutorial | None | Voiceover |

## What I Learned

- Define a minimum viable product early, and cut features before the deadline forces you to.
- Test on the headset often. Small errors in scale, rotation or position can break a VR experience, and fixing them takes longer than expected.
- Give each part of the Unity project a clear owner to avoid overlap, and commit regularly so work is backed up on GitHub.

## Running the Project

1. Install Unity 6000.3.13f1 from Unity Hub. Android build support is needed to build for a headset.
2. Clone the repository and add the project folder in Unity Hub.
3. Open `Assets/Scenes/IntroScene.unity` and press Play. Without a headset, use the XR Device Simulator from the XR Interaction Toolkit samples included in the project.
4. To play on a headset, switch the build target to Android and build to a device that supports OpenXR or Oculus.


https://github.com/user-attachments/assets/a5095063-eddd-4520-ad54-25a52dab4535



