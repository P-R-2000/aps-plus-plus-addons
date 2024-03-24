# Fireworks Addon
This highly-customizable addon allows you to add fireworks in your server!
![fireworks image](https://github.com/P-R-2000/aps-plus-plus-addons/blob/main/fireworks/image.jpg?raw=true)
Fireworks get spawned every time an entity dies.
# Setup
## Basic Setup
To use this addon with the default settings:
1. Download `fireworks.js` and move it into the `server/modules/definitions/addons` folder.
2. In your `server/config.js` file add `FIREWORKS: true,` to enable the addon.
## Advanced Setup
You can customize the firework settings using config's FIREWORK object property.
### Properties
| Property     | Type     | Description                                                                                                                                                             | Default                                           | Example                                        |
|--------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------|------------------------------------------------|
| SHAPES       | array    | Possible fireworks shapes.                                                                                                                                              | `[0, 3, 4, /*STAR*/]`                             | `[0,8,20]`                                     |
| COLORS       | 2d array | Possible fireworks colors. The length of the color array MUST NOT be higher than the max count.                                                                         | `[[10, 12], [12, 2], [10, 28], [14, 5], [1, 11]]` | `[[20, 21, 22, 23, 24], ["orange", "yellow"]]` |
| MIN          | int      | The minimum count of fireworks.                                                                                                                                         | `6`                                               | `4`                                            |
| MAX          | int      | The maximum count of fireworks.                                                                                                                                         | `22`                                              | `6`                                            |
| SPEED        | float    | The firework speed.                                                                                                                                                     | `7`                                               | `10`                                           |
| RANGE        | float    | The firework range.                                                                                                                                                     | `25`                                              | `20`                                           |
| SIZE         | float    | The firework size.                                                                                                                                                      | `5`                                              | `12`                                           |
| HEALTH       | float    | The firework health.                                                                                                                                                    | `10`                                              | `100`                                          |
| DAMAGE       | float    | The firework damage.                                                                                                                                                    | `10`                                              | `20`                                           |
| ENTITY_TYPES | array    | The entity types which death spawns fireworks                                                                                                                           | N/A                                               | `["bullet", "drone", "food"]`                  |
| CHECK_ENTITY | function | Checks if the entity's death should spawn fireworks. Returns true if the fireworks should be spawned. NOTE: If CHECK_ENTITY exists, then ENTITY_TYPES won't be checked. | N/A                                               | `e => e.isPlayer \|\| e.isBot`                 |
|SPAWN_EVERY_MS| int      | Spawns fireworks in a random position every n milliseconds.           | N/A                                               | `100`                                        |
