# Robots 2026 – Virtual Reality Game

A virtual reality quiz game built in Unity with C#. The player talks to four robots, hears each robot's opinion on a question, and then answers on a tablet. The game has 5 questions and ends on a win or lose screen. It was built by a team of five (3 art students and 2 computer science students) and demonstrated in class.

## How It Plays

1. The game starts on a welcome screen.
2. Each question appears on a tablet.
3. The tablet stays locked until the player has interacted with all 4 robots. Selecting a robot with the ray interactor displays that robot's opinion on the current question.
4. Once all 4 robots have been consulted, the tablet unlocks and the player answers.
5. After the last question, the game moves to a win or lose scene. `[PLACEHOLDER: what decides win versus lose]`

## Features

- 5 quiz questions, with robot opinions that change for each question.
- Ray-based interaction using Unity's XR Interaction Toolkit.
- Tablet lock that forces the player to engage with every robot before answering.
- Scene flow from the welcome screen to each question, then to the win or lose scene.
- Score tracking and player locomotion.

## Tech Stack

- Unity `[PLACEHOLDER: Unity version]`
- C#
- XR Interaction Toolkit and XR Hands
- Target headset: `[PLACEHOLDER: for example Meta Quest, or leave out]`

## My Contributions

I was one of the two programmers on the team. I built:

- the quiz questions and the per-question robot opinions displayed when a robot is selected
- the ray interactor setup, and testing that interactions worked properly
- the tablet lock that requires all 4 robots to be consulted before answering
- the transitions from the welcome screen through each question to the win and lose screens

The other programmer built the scoring system and player locomotion. The three art students created the visual assets. `[PLACEHOLDER: confirm what the art team made]`

## Running the Project

1. Install Unity `[PLACEHOLDER: version]` with the required XR modules.
2. Clone the repository and open it as a Unity project.
3. Open the welcome scene `[PLACEHOLDER: scene name]` and press Play, or build to your headset.

## Team

`[PLACEHOLDER: list all 5 team members and their roles]`
