# Reflection

## User Scenario 1

Map Outline:

- `c_intro_guitar_wiring.dita`
- `t_prerequisites.dita`
- `t_prep_materials.dita`
- `r_wiring_components.dita`
- `r_soldering_details.dita`
- `t_connect_hot_wires.dita`
- `t_connect_capacitor.dita`
- `t_ground_the_circuit.dita`
- `t_install_the_circuit.dita`
- `t_test_the_circuit.dita`
- `c_conclusion_guitar_wiring.dita`

The user in scenario 1 is a complete beginner, so a near full wiring guide is a necessity. This one was a bit tough to navigate because we're concerned with the length, but to complete a full rewire every step is necessary. It would be easy to split up the guide into smaller ones if we are making maps for the guides specifically (one for prepping materials, one for wiring, one for troubleshooting), but given the map is based on an overarching user goal, it should probably include everything save for troubleshooting, which is how we approached it. 

This map, when filtered for novice information, outputs a detailed and comprehensive procedure that covers everything this user would need to know. 

> This is the one we're most iffy on in regards to amount of, so feedback and suggestions would be greatly helpful.

Upon completing this guide, the user will have been equipped with the knowledge and skills to do this again on their own (even able to use the expert guide shown in scenario 2, if needed) and translate them to different guitar wiring projects that have different circuit layouts.

## User Scenario 2

Map outline:

- `c_intro_guitar_wiring.dita`
- `t_connect_humbucker.dita`
- `t_connect_hot_wires.dita`
- `t_connect_capacitor.dita`
- `t_ground_the_circuit.dita`
- `t_test_the_circuit.dita`

The in user scenario 2 is an expert when it comes to terminology and has some experience with wiring other things (their pedalboard). In many cases, the wiring diagrams will provide sufficient instruction. 

The map also capitalizes on assumed knowledge: since the user is experienced and since they are just swapping parts, information such as comprehensive prerequisites and instructions for installing the circuit are not needed. The map only covers the major parts that the user may need assistance with. 

In the cases where the user does need assistance, many substeps are filtered out given the user will know how to conduct the step given the command and diagram. Some alternate steps are given for expert audiences only to streamline the process, such as in `t_test_the_circuit.dita` where expert users can simply tap the humbucker with a screwdriver to test for sound instead of playing a song through the pickup (expert users will know what specific sound details to look out for that are easier to spot with the latter method). 

The main consideration for this scenario was preserving detailed diagrams, ensuring none get filtered out.

## User Scenario 3

- `c_guitar_wiring_troubleshooting_overview.dita`
- `t_weak_or_no_sound_parent.dita`
  - `t_test_faulty_humbucker_output_jack.dita`
  - `t_check_cold_solder_joints.dita`
  - `t_fix_miswired_connection.dita`
  - `t_verify_pickup_grounding_connection.dita`
  - `t_replace_damaged_potentiometers.dita`
    - `r_soldering_details.dita`
    - `t_connect_hot_wires.dita`
    - `t_ground_the_circuit.dita`

This user scenario falls more into the "intermediate" category than anything else. The map assumes the user has already installed new electronics but are encountering an error with the sound: there is no sound. This limits the scope to just that issue, so this troubleshooting map only concerns itself with related topics. There are no topics related to circuit humming or pot knob direction. 

This map has the user work through five child troubleshooting tasks to narrow down the problem. If it's a problem with the humbucker, the user stops after the first child task; if it's a problem with the solder joints, the user stops after the second child task, and so on. If none of those work and they make it to the end of the troubleshooting steps, it must be a faulty potentiometer(s).

Given that, the map reuses three topics to set the user on the right track when they go to replace the potentiometers. Those final three topics also serve the previous child task topics as their steps can be used to fix miswired connections or grounding issues if the user is confused on how to do that properly. 

Since they have already wired things, there's no need for steps on prepping materials, testing, or installing.

