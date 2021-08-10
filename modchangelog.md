
###### Logging the changes

Script | Line | From | To | Effect
------------ | ------------- | ------------- | ------------- | -------------
RobotScript.cs | 543 | `float kFlySpeed = 10.0f` | `float kFlySpeed = 6.0f` | Shock (Flying) Drone speed at 60%
RobotScript.cs | 317 | `Time.deltaTime * 100.0f` | `Time.deltaTime * 60.0f` | Turret rotational speed while idle at 60%
AimScript.cs | 2220 | `if(old_vel.y < -8.0f){` | `if(old_vel.y < -10.0f){` | Player wont die falling from single story unless jumping.
RobotScript.cs | 81 | `float kMaxRange = 20.0f;` | `float kMaxRange = 15.0f;` | All drone target range decreased to 75%
BulletPileScript.cs | 20 | `int num_bullets = UnityEngine.Random.Range(1,6);` | `int num_bullets = UnityEngine.Random.Range(2,8);` | Bullets in pile now between 2 and 6
RobotScript.cs | 77 | `float kAlertDelay = 0.6f;` | `float kAlertDelay = 0.6f;` | Turrets will take twice as long to fire at player if spotted
*AimScript.cs | 487 - 488 | `int num_start_bullets = UnityEngine.Random.Range(0,10);` | `GunScript gun_script = GetGunScript(); int max_rounds = 7; int extra_rounds = UnityEngine.Random.Range(1, 8); if (gun_script.HasGunComponent(GunAspect.REVOLVER_CYLINDER)) { max_rounds = 6; extra_rounds = UnityEngine.Random.Range(3, 8); } else if (gun_script.HasGunComponent(GunAspect.FIRE_MODE)) { max_rounds = 17; extra_rounds = 0; }int num_start_bullets = max_rounds + extra_rounds; ` | Player will start with enough bullets to fill chamber / magagine and possibly get extra unless starting weapon is the glock`
optionsmenuscript.cs | 62 / 73-76 | ` ` | `GunLock();` / `public void GunLock() {
      PlayerPrefs.SetInt("lock_gun_to_center", 1);
    }`  | Gun Lock toggle is on by default in menu





\* Subject to change
