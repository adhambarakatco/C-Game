# C++ Shooter Game: Fusion of Pac-Man and Metal Slug

## Overview

This is a 2D console-based shooter game that combines elements from the classic games Pac-Man and Metal Slug. The objective of the game is to navigate through a 15x15 grid, hunting down all the monsters without dying. Players control a hero character, which can be chosen from different types, each with unique abilities, while engaging in combat with various monsters using a range of weapons.

## Game Features

- **Heroes and Monsters**: Players can select between two hero classes—MedicHero and DemolitionHero—each offering unique gameplay mechanics.
  - **MedicHero**: Has a healing ability to restore health.
  - **DemolitionHero**: Can wield two weapons simultaneously.
- **Monsters**: The game includes different types of monsters, each with distinct characteristics, such as GhostMonster and TankMonster.
  - **GhostMonster**: Can temporarily become invisible.
  - **TankMonster**: Has an additional shield attribute to absorb damage.
- **Weapons**: The game features different weapons with specific attributes and capabilities.
  - **Pistol**: 16 bullets, range of 2, and damage of 30.
  - **Bazooka**: 4 bullets, range of 8, and damage of 150.
  - **Rifle**: 30 bullets, range of 4, and damage of 20.

## Game Mechanics

- **Movement and Combat**: The player moves the hero across the grid to engage with monsters, collect items, and strategically use abilities.
  - **Move**: Use 'w', 's', 'a', 'd' keys to move the hero across the grid.
  - **Attack**: Fire weapons to attack monsters within range.
  - **Special Abilities**: Each hero and weapon has a unique special ability that adds strategic depth to gameplay.
- **Map Elements**: The game map is a 15x15 grid containing:
  - **Ammo**: Collect ammo to refill the hero's weapons.
  - **Potions**: Restore health points.
  - **Monsters**: Eliminate all monsters to win the game.
- **Operators Overloading**: The game includes overloaded operators for interacting with items and monsters, adding ammo, using potions, and engaging in combat.

## Classes Overview

### Object Class
- Base class for all other game elements.

### Character Class
- Base class for the **Hero** and **Monster** classes.

### Hero Class
- Represents the player-controlled character with subclasses for **MedicHero** and **DemolitionHero**.

### Gun Class
- Represents different types of guns, each with unique capabilities. Includes subclasses **Pistol**, **Bazooka**, and **Rifle**.

### Monster Class
- Represents enemies on the grid, with subclasses **GhostMonster** and **TankMonster**.

### Item Class
- Represents collectible items such as **Ammo** and **Potions**.

### Game Class
- Manages the overall game mechanics, including the game grid, hero interactions, and game flow.

## Game Flow
1. **Hero Selection**: The player chooses between MedicHero and DemolitionHero.
2. **Weapon Selection**: The player selects the hero's weapon (or two weapons for DemolitionHero).
3. **Gameplay**: Navigate the grid, defeat all monsters, collect items, and avoid losing health to reach the objective.
   - Use the `move` function to navigate.
   - Use `FireGun` to shoot in the specified direction.
   - Use `useGunSpecial` to activate special weapon abilities.
   - Monsters will respawn and disappear at set intervals, creating a dynamic challenge.
4. **Game Over Conditions**:
   - The game ends if the hero loses all health or if all monsters are eliminated.

## Controls
- **Movement**: `w` (up), `s` (down), `a` (left), `d` (right)
- **Attack**: Input the direction to shoot after selecting a weapon.
- **Special Abilities**: Trigger special hero or weapon abilities.

## Compilation and Execution
- This project contains header files for each class, alongside a single source file implementing the game logic.
- To compile and run the game, ensure you have a C++ compiler like `g++`.
- Use the following commands:
  ```sh
  g++ main.cpp -o ShooterGame
  ./ShooterGame
  ```

## Installation and Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/YourUsername/YourRepository.git
   ```
2. Navigate to the project directory:
   ```sh
   cd YourRepository
   ```
3. Compile and run the game using the provided commands.

## Future Improvements
- **AI for Monsters**: Adding simple AI to allow monsters to chase the hero.
- **Additional Levels**: Increase grid size and introduce new types of monsters and challenges.
- **Graphics**: Add a graphical user interface for enhanced gameplay.

## Contributing
Contributions are welcome! Feel free to submit issues or pull requests for improvements or bug fixes.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

