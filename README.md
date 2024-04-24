# MAMMOTH: Mid-Air Mesh-based Modulation Optimization Toolkit for Haptics
The toolkit enables auto-generated ultrasound haptics for mid-air hand interactions using the 2-opt algorithm and dynamic frequency modulation.

## Dependencies
The software can be modified for other software and hardware. The plugin has been tested with the following.

#### Software
- Ultraleap Tracking Service 5.13
  - Unity Plugin "Tracking"
  - Requires ServiceProvider
- UltraleapHapticsWithExample-3.0.0-beta.10
  - Only tested with this version. May require slight adaption for newer versions.
- Tested in Unity 2021.3.1f1

#### Hardware
- Ultrahaptics Stratos Explore
- Leap Motion

## Instructions
#### Add the following to your Unity project:
1. MAMMOTH Plugin
2. Ultraleap Tracking Service (see above)
3. Ultrahaptics (see above)

#### Add the following to a scene:
  1. ServiceProvider
  2. DiscretizedHand Prefab
      - Set the ServiceProvider values in the inspector for the two HandBinder components on LoPoly_Rigged_Hand_Left and LoPoly_Rigged_Hand_Left
  4. Add MammothRenderer script to a Gameobject in the scene (e.g., ServiceProvider)
      - Set the ServiceProvider value in the inspector
  5. Add a meshed object with a collider (e.g., 3D Sphere or Cube)
      - Attach MammothInteractable script to the gameobject
      - Set the MammothRenderer value in the inspector
  6. Run the scene

# Contact
TBD
You can find more information in the CHI '24 EA paper MAMMOTH: Mid-Air Mesh-based Modulation Optimization Toolkit for Haptics (to be published)
