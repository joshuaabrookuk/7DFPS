
###### Logging the changes

Script | Line | From | To | Effect
------------ | ------------- | ------------- | ------------- | -------------
RobotScript.cs | 543 | `float kFlySpeed = 10.0f` | `float kFlySpeed = 6.0f` | Shock (Flying) Drone speed at 60%
RobotScript.cs | 317 | `Time.deltaTime * 100.0f` | `Time.deltaTime * 60.0f` | Turret rotational speed while idle at 60%
AimScript.cs | 2220 | `if(old_vel.y < -8.0f){` | `if(old_vel.y < -10.0f){` | Player wont die falling from single story unless jumping.






rotation_y.target_state += Time.deltaTime * 60.0f;  317:  // rotation speed of the gun pivot while idle - Yoshito
