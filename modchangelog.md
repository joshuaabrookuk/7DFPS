
###### Logging the changes

Script | Line | From | To | Effect
------------ | ------------- | ------------- | ------------- | -------------
Robotstript.cs | 543 | `float kFlySpeed = 10.0f` | `float kFlySpeed = 6.0f` | Shock (Flying) Drone speed at 60%
Robotstript.cs | 317 | `Time.deltaTime * 100.0f` | `Time.deltaTime * 60.0f` | Turret rotational speed while idle at 60%







rotation_y.target_state += Time.deltaTime * 60.0f;  317:  // rotation speed of the gun pivot while idle - Yoshito
