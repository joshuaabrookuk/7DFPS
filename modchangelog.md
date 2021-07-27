
###### Logging the changes

Script | Line | From | To | Effect
------------ | ------------- | ------------- | ------------- | -------------
RobotScript.cs | 543 | `float kFlySpeed = 10.0f` | `float kFlySpeed = 6.0f` | Shock (Flying) Drone speed at 60%
RobotScript.cs | 317 | `Time.deltaTime * 100.0f` | `Time.deltaTime * 60.0f` | Turret rotational speed while idle at 60%
AimScript.cs | 2220 | `if(old_vel.y < -8.0f){` | `if(old_vel.y < -10.0f){` | Player wont die falling from single story unless jumping.
RobotScript.cs | 81 | `float kMaxRange = 20.0f;` | `float kMaxRange = 15.0f;` | All drone target range decreased to 75%
BulletPileScript.cs | `int num_bullets = UnityEngine.Random.Range(1,6);` | `int num_bullets = UnityEngine.Random.Range(2,8);` | Bullets in pile now between 2 and 8
