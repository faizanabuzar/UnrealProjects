# S05 Testing Grounds - First Person Shooter

A first-person shooting game built with Unreal Engine 4.19, featuring infinite terrain generation, AI-controlled NPCs, and dynamic gameplay mechanics.

## Features

### Core Gameplay
- **First-Person Shooter Mechanics**: Complete FPS controls and shooting system
- **Projectile-Based Combat**: Ball projectile system with physics-based interactions
- **Infinite Terrain Generation**: Procedurally generated world using tile-based system
- **AI NPCs**: Intelligent non-player characters with patrol behavior
- **Dynamic Environment**: Grass generation and environmental details

### Technical Features
- **Modular Architecture**: Clean separation of Player, NPC, Weapons, and Terrain systems
- **AI Behavior Trees**: NPCs with waypoint-based patrol routes
- **Object Pooling**: Efficient actor pool system for performance optimization
- **Custom Game Modes**: Specialized game modes for different gameplay scenarios

## Project Structure

```
S05TestingGrounds/
├── Content/
│   ├── Player/           # Player character assets and blueprints
│   ├── Weapons/          # Weapon models, animations, and effects
│   ├── NPC/             # AI character assets and behavior trees
│   ├── Terrain/         # Terrain generation and environmental assets
│   ├── Levels/          # Game levels and maps
│   └── TestingGroundPack/ # Additional game assets
├── Source/
│   └── S05TestingGrounds/
│       ├── Player/      # First-person character implementation
│       ├── Weapons/     # Gun and projectile systems
│       ├── NPC/         # AI patrol and waypoint systems
│       ├── Terrain/     # Infinite terrain and grass generation
│       └── Character/   # Base character classes
└── Config/              # Game configuration files
```

## System Requirements

- **Engine**: Unreal Engine 4.19
- **Platform**: Windows (primary), with potential for cross-platform deployment
- **Dependencies**: AIModule, Engine (Core UE4 modules)

## Getting Started

### Prerequisites
- Unreal Engine 4.19 installed
- Visual Studio 2017 or later (for C++ development)
- Windows 10 or later

### Setup Instructions
1. Clone or download the project
2. Right-click on `S05TestingGrounds.uproject` and select "Generate Visual Studio project files"
3. Open `S05TestingGrounds.sln` in Visual Studio
4. Build the solution (Build → Build Solution)
5. Launch the project by opening `S05TestingGrounds.uproject` in Unreal Engine

### Controls
- **WASD**: Movement
- **Mouse**: Look around
- **Left Click**: Shoot
- **Space**: Jump (if implemented)

## Key Components

### Player System
- **FirstPersonCharacter**: Main player controller with FPS mechanics
- **Mannequin**: Base character class for shared functionality

### Weapons System
- **Gun**: Primary weapon implementation
- **BallProjectile**: Physics-based projectile system

### AI System
- **PatrolRoute**: Defines patrol paths for NPCs
- **ChooseNextWaypoint**: AI behavior for waypoint selection

### Terrain System
- **Tile**: Individual terrain tile management
- **GrassComponent**: Procedural grass generation
- **InfiniteTerrainGameMode**: Manages infinite world generation

### Optimization
- **ActorPool**: Object pooling system for performance

## Development Notes

This project demonstrates several key game development concepts:
- Component-based architecture
- AI behavior implementation
- Procedural content generation
- Performance optimization techniques
- Physics-based gameplay mechanics

## Contributing

When contributing to this project:
1. Follow the existing code structure and naming conventions
2. Test all changes in both Blueprint and C++ contexts
3. Ensure compatibility with Unreal Engine 4.19
4. Document any new features or significant changes

## License

[Add your license information here]

## Acknowledgments

Built as part of learning Unreal Engine 4 game development, focusing on first-person shooter mechanics and procedural world generation.
