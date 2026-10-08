# Robots 2026 – Virtual Reality Game

A virtual reality quiz game built in Unity with C#. The player investigates the story of the fictional company Robot Corp by asking four robots for their opinions, then answers questions on a tablet. It was built by a team of five (3 art students and 2 computer science students) and demonstrated in class.

## How It Plays

1. **Intro:** the game opens with an audio introduction, then loads the main scene. Press `S` on the keyboard to skip the intro.
2. **Start:** press Start on the tablet to begin the quiz.
3. **Consult the robots:** each question appears on the tablet with four answers, but the answers are locked. Point at a robot's name tag with the ray interactor and click it to hear that robot's opinion on the current question. The robots are PIPER, SAM, HELO and GIDE.
4. **Answer:** once all four robots have been consulted, the answers unlock. Each answer is worth points, and the correct answers are worth the most.
5. **Repeat:** the robots reset for the next question. After all 5 questions, the game loads the winner scene if the score reaches 70 points, and the loser scene otherwise.

The five questions ask about Robot Corp: when and by whom it was founded, its mission, what caused the 2021 Shutdown, and what the company is hiding.

## Features

- 5 quiz questions, each with a separate opinion from each of the 4 robots.
- Ray-based VR interaction using Unity's XR Interaction Toolkit.
- Tablet lock that keeps answers disabled until the player has consulted all 4 robots.
- Score tracking with a win threshold.
- Four scenes: `IntroScene`, `MainScene`, `WinnerScene` and `LoserScene`.
- Questions stored as Unity `ScriptableObject` assets (`Assets/Questions`), so they can be edited without changing code.

## Tech Stack

- Unity 6 (6000.3.13f1) with C#
- XR Interaction Toolkit 3.3.1 and XR Hands 1.7.3
- OpenXR 1.16.1 and the Oculus XR Plugin 4.5.4
- Unity Input System and TextMeshPro

## My Contributions

I was one of the two programmers on the team. I built:

- the quiz questions and the per-question robot opinions displayed when a robot is selected
- the ray interactor setup, and testing that the interactions worked properly
- the tablet lock that requires all 4 robots to be consulted before answering
- the transitions from the intro through each question to the win and lose scenes

The other programmer built the scoring system and player locomotion. The three art students created the robots and the environment.

## Running the Project

1. Install Unity 6000.3.13f1 from Unity Hub. Android build support is needed to build for a headset.
2. Clone the repository and add the project folder in Unity Hub.
3. Open `Assets/Scenes/IntroScene.unity` and press Play. Without a headset, use the XR Device Simulator from the XR Interaction Toolkit samples included in the project.
4. To play on a headset, switch the build target to Android and build to a device that supports OpenXR or Oculus.
