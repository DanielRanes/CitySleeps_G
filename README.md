CitySleeps_G

A C# Windows Forms application built to assist a gamemaster/moderator in running a social deduction party game (similar to Mafia/Werewolf), where players are secretly assigned hidden roles and the moderator manages a night/day cycle of actions and eliminations.

About the project

I built this for fun, to practice C# and .NET, and to make it easier to run this game with friends — instead of the moderator keeping track of everyone's role, HP, and abilities by memory or on paper, the app handles the bookkeeping.

How it works

Setup (Form1)

The moderator sets the number of players.
Roles are randomly shuffled and assigned as each player's name is entered — every player gets a unique, hidden character with its own ability.
Once everyone is added, the moderator can view the full player/role list before starting the game.

Gameplay (Form2)

The game alternates between Night and Day phases.
During the night, the moderator wakes up each role in a fixed order, and uses their ability on a chosen target (e.g. the Killer deals damage, the Doctor heals, the Detective can expose or eliminate a Killer).
During the day, players vote to eliminate a suspect.
The app tracks each player's HP, who's still alive, which roles have already acted that night, and declares a winner once either the killers or the townspeople gain the upper hand.
A live data grid shows the status of all players (HP, night-active, acted, blocked) for the moderator's reference.
Roles (examples)
Gyilkos / Keresztapa (Killer / Godfather) — deal damage to a target at night
Orvos (Doctor) — heals a target
Felugyelo (Detective) — investigates/blocks a target, can instantly eliminate a Killer
Kislany (Little Girl) — can secretly observe the killers at night
...and several more, each with a unique night ability
Tech
C# / .NET, Windows Forms
Two main forms: player/role setup, and the night/day game loop
Status

A personal side project built for practice and for playing with friends; not actively maintained, but feel free to open an issue with suggestions or bugs.
