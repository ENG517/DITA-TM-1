# DITA Topic Model - Enter Title Here

This repo contains a DITA topic model (TM) ...

## Authors

- Enter names here

## Project Maps

### User Scenario 1:

Jordan is a hobby guitarist who has been playing for a few years. They mostly play at home and occasionally jam with friends. Their main guitar is a Les Paul Jr. they bought used. It plays well, but the volume knob has become scratchy and cuts in and out when they roll it. Jordan also wants a smoother taper so the volume roll-off feels more natural while playing.

Jordan doesn’t have a lot of experience with electronics, but they’ve done basic maintenance before—string changes, pickup height adjustments, and installing a new output jack with help from a YouTube tutorial. They’re comfortable with a soldering iron but still double-check every step.

#### Goal

Replace the existing volume and tone pots with new 250k pots that offer smoother control and better reliability.

Map Outline (Novice):
- c_intro_guitar_wiring.dita
- t_prerequisites.dita
- t_prep_materials.dita
- r_wiring_components.dita
- r_soldering_details.dita
- t_connect_hot_wires.dita
- t_ground_the_circuit.dita
- t_install_the_circuit.dita
- t_test_the_circuit.dita

### User Scenario 2: ...

Alex is an experienced guitarist who has been playing and performing for over a decade. They’re familiar with tone shaping concepts, but they’ve never actually modified a guitar’s internal wiring before. They’re comfortable with soldering because they build their own pedal kits, but guitar wiring still feels unfamiliar territory.

Alex owns an Epiphone Les Paul Jr. they use as a reliable backup guitar. They want to add a new humbucker, a new volume pot, and a no-load tone pot for a more open top-end when rolled up.

#### Goal

Install a new a humbucker, a set of 250k pots, and a 0.022µF capacitor, ensuring clean solder joints and maintaining signal integrity.

Map Outline (Expert):
- c_intro_guitar_wiring.dita
- t_prerequisites.dita
- t_connect_humbucker.dita
- t_connect_hot_wires.dita
- t_ground_the_circuit.dita
- t_test_the_circuit.dita

### User Scenario 3: ...

Casey is an intermediate guitarist who’s been playing for several years. They’re comfortable doing simple guitar setup work—adjusting action, restringing, adjusting pickup height, and they recently felt confident enough to replace the electronic components in their Les Paul. They installed new 250k pots, a new capacitor, and a fresh output jack.

The installation seemed to go smoothly. Casey followed a wiring diagram and took reference photos before desoldering. However, after reassembling the guitar, plugging into their practice amp, and testing the controls, they notice an issue:

#### Problem

The guitar produces no sound and the volume knob does nothing.

Casey isn't sure whether the issue is a wiring mistake, a cold solder joint, or a mis-grounded connection. They know how solder joints should look and how components interact, but they don’t have deep experience diagnosing guitar wiring problems.

#### Goal

Identify and correct the wiring or grounding issue causing the volume control to be bypassed or ineffective.

Map Outline:
- c_guitar_wiring_troubleshooting_overview
- c_filename.dita (File title)
- t_weak_or_no_sound_parent.dita
  - t_check_cold_solder_joints.dita
  - t_fix_miswired_connection.dita
  - t_verify_pickup_grounding_connection.dita
- t_replace_damaged_potentiometers.dita
  - r_soldering_details.dita
  - t_connect_hot_wires.dita
  - t_ground_the_circuit.dita

## Folders &amp; Files

- `assets`: Contains all assets used within the TM.
- `concepts`: Contains all concept topics.
- `references`: Contains all reference topics.
- `tasks`: Contains all task topics.
- `shared`: Contains all topic files that are shared across multiple maps.
- `out`: Contains all output folders.
- `themes`: Contains `.yaml` style configuration files.
- **Skeleton files**: All topic folders contain a single "skeleton" topic file for you to copy, whenever you need to quickly create a new file.
- `.keep` **files**: Ignore these files. They ensure that any empty folders are tracked by git. 
- `.gitignore`: This file tells git which files to ignore in the repo. You can leave this one be.

## Filenaming Conventions

- Task Topics: `t_verb_verbobject.dita`
- Concept Topics: `c_nounphrase.dita`
- Reference Topics: It varies, but something akin to `r_types_of_nounphrase.dita`
- Dita Maps: `_modelname.ditamap`

## Building Outputs Manually with the Command Line

See the DITA-OT user guide about how to generate output: [https://www.dita-ot.org/dev/topics/build-using-dita-command](https://www.dita-ot.org/dev/topics/build-using-dita-command)

### Sample DITA Commands

#### Help

To see all of the commands and parameters, use the following command:

```
dita --help
```

#### DITA options and arguments

```
-f == dita output format
-i == dita input map file
-o == dita output directory
-D&lt;property&gt;=&lt;value&gt; == add custom args
    with particular values to dita transformation
-filter &lt;file&gt; == filter and flagging file
```

#### Create an HTML5 site

```
dita -f html5 -i 'url/to/your/wanted.ditamap' \
  -o 'url/to/your/output/folder' \
```

#### Create an HTML5 site with a custom CSS file

```
dita -f html5 -i 'url/to/your/wanted.ditamap' \
  -o 'url/to/your/output/folder' \
  -Dargs.cssroot='url/to/your/assets/folder' \
  -Dargs.css='${cssroot}/your-custom-css-file.css' \
  -Dargs.csspath='css' \
  -Dargs.copycss='yes'
```

#### Create a PDF

```
dita -f pdf -i 'url/to/your/wanted.ditamap' \
  -o 'url/to/your/output/folder' \
```
