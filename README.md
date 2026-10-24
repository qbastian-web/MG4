# MG4
## Devlog
The FloatAnimation script makes use of four member variables: _moveSpeed and _switchSpeed, which can be set in the Unity editor, and _up and _timer, which cannot. The script moves the GameObject up and down through its Update() method which utilizes the four member variables: It first checks _up to determine if it should be moving upward or downward, then translates the GameObject the appropriate amount, which is dependent on Time.deltaTime and _moveSpeed. Afterwards, it decreases _timer by Time.deltaTime (which was initally set to _switchSpeed in the script's Start() function) and checks if it is currently less than zero; if so, _timer is set back to _switchSpeed and the value of _up is swapped. The variables of this function effectively represent the speed at which the object moves, the time in seconds it takes for the object to switch directions, what direction the object is currently traveling in, and how much time left the object has before it switches directions again.

## Open-Source Assets
- [Quirky animal 3D models](https://assetstore.unity.com/packages/3d/characters/animals/quirky-series-free-animals-pack-178235)
- [City 3D models](https://assetstore.unity.com/packages/3d/environments/simplepoly-city-low-poly-assets-58899)
- [Bite sound effect](https://freesound.org/people/Jofae/sounds/353067/)