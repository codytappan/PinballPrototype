# PinballPrototype
Learning project for Unity based game developement

# Style Guide
## Project Organization
### Directory Structure
The top level project is set by Unity, where possible we aim to avoid creating new top level directories. Directories and files are named using `PascalCase`. Avoid spaces, underlines, and hyphens.

Assets specific to this project are organized by content type under the `Assets/ProjectName` dir. Any third party assets will be placed directly under `Assets` by default.

`Assets/ProjectName/Art` contains all visual art assets like textures, animations, and models
`Assets/ProjectName/Audio` contains all audio art assets like sound effects, and music
`Assets/ProjectName/Code` contains all code assets like scripts, and shaders
`Assets/ProjectName/Level` contains all game design assets like scenes, UI, and prefab objects

Testing and work in progress assets should be located under `Assets/Sandbox`, should follow the same subdir heirarchy, and should never be used in production code until finalized.

## Coding Standards
Following Google's C# style guide here: https://google.github.io/styleguide/csharp-style.html

Wherever it makes sense logically, organize elements of each Level in to child objects of an empty GameObject for convenience. For example, Background, Environment, Projectiles, Player all make sense as high level objects that may contain many child objects.

Similarly, game behaviors should be grouped in to discrete subsystems. Collider, Renderer, Shooter, all make sense as logically separated behavioral systems to be used by GameObjects
