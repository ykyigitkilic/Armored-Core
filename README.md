# Armored-Core
"""
Overview
This is a console-based mech combat game inspired by the Armored Core series. Players build custom mechs from a variety of parts and weapons, select a subclass, and battle against AI or another player. The game is written in Python and uses JSON for part data and pickle for save files.

Game Structure
main.py: Entry point, handles game flow (new game, load, multiplayer, battles, hangar).
game_classes.py: Defines core classes: Part, Mech, SubClass, and the list of available subclasses.
game_functions.py: Contains functions for loading parts, selecting parts/weapons, handling turns, enemy AI, hangar upgrades, saving/loading, and more.
parts.json: Database of all available parts and weapons.
Gameplay Flow
Start: Choose New Game, Load Game, or Multiplayer.
Mech Building: Select subclass, then pick head, torso, generator, legs, arms, and 4 weapons.
Battle Loop: Face off against AI enemies (or another player in multiplayer). Each turn, choose to attack (with a weapon), evade, or wait (recover energy).
Enemy AI: Randomly chooses to attack or evade, based on available energy.
Hangar: After each victory, access the hangar to upgrade parts (buffed versions), get new weapons, repair, or save/exit.
Progression: Each battle increases the enemy count; player HP and energy are restored after hangar.

Features
Parts System: Wide variety of weapons and parts, each with stats (damage, energy cost, HP, weight, power).
Subclasses: Four subclasses, each with a unique bonus (damage, HP, energy, or evasion).
Turn-Based Combat: Simple but strategic, with energy management and evasion.
Hangar Upgrades: After each battle, players can swap to improved parts and weapons.
Save/Load: Progress can be saved and loaded.
Multiplayer: Two players can build mechs and battle in hotseat mode.

Code Quality & Design
Modular: Good separation of concerns between game logic, data, and classes.
Extensible: Easy to add new parts, weapons, or subclasses via JSON and class lists.
Readable: Code is clear, with descriptive function and variable names.
Error Handling: Basic input validation and error messages.
Serialization: Uses pickle for saving/loading, with subclass restoration logic.

Strengths
Customization: Lots of parts and weapons for varied builds.
Replayability: Randomized enemy builds and hangar upgrades.
Strategic Depth: Energy management, evasion, and subclass bonuses add tactical choices.
User Feedback: Status displays and clear prompts guide the player.
Conclusion
This is a solid foundation for a turn-based mech combat game, with strong customization and a clear, modular codebase. With further development, especially in AI, progression, and combat depth, it could become a compelling console strategy game for fans of the genre.
"""
