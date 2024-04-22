# Black Hole Addon
This addon adds a black hole tank that has a gravitational attraction.
![Black hole clip](https://github.com/P-R-2000/aps-plus-plus-addons/blob/main/blackHole/clip.webm)
## Setup
To use this addon download [this file](https://github.com/P-R-2000/aps-plus-plus-addons/blob/main/blackHole/blackHole.js) and move it into the `server/modules/definitions/addons` folder.
## Customization
You can change some constants in `blackHole.js` to customize how the black hole behaves.
| Constant             | Type               | Description                                                                          |
|----------------------|--------------------|--------------------------------------------------------------------------------------|
| range                | float              | The range of the black hole attraction (the maximum distance of affected entities).  |
| mass                 | float              | The mass of the black hole. Increases the force of the attraction.                   |
| G                    | float              | The gravitational constant.                                                          |
| sizeChangeMultiplier | float              | Increases/decreases the size of the attracted entities.                              |
| ignored              | array of functions | Array of functions that return true if the entity should be ignored (not attracted). |
| ignoredTypes         | array of strings   | Array of entity types that should be ignored (not attracted).                        |