# raveniung

Keyboard designed with ergogen, heavenly inspired by the reviung34

### First time setup

* Install ergogen: `npm install -g ergogen`
* Get footprints from ceoloide: `git clone https://github.com/ceoloide/ergogen-footprints ergogen/footprints/ceoloide`
* For case build install `npm install -g @jscad/cli`

## v0.1 for Cirque Trackpad

### Build

```bash
cd ergogen
cp config-v0.1.yaml config.yaml
ergogen .
```

or for building including the left case:

```bash
ergogen . && npx @jscad/cli@1 output/cases/LeftCase.jscad -of stla
```

### Notes

* mirror right case and cirque holder!

## v0.2 for Azoteq TPS65 touchpad

### Build

```bash
cd ergogen
cp config-v0.2.yaml config.yaml
ergogen .
```

or for building including the cases:

```bash
ergogen . && npx @jscad/cli@1 output/cases/Case.jscad -of stla && npx @jscad/cli@1 output/cases/TouchpadCase.jscad -of stla
```

### TODO

## Notes

* Mount TPS65 so that FFC connector is further away from PCB connector. On left side when looking from bottom
* Use straight FFC cable (both blues on same side)
* Ply 90 degrees in the middle of the touchpad PCB
* Use FFC connector with connections on bottom (Verify before soldering!)

### Laser cutting (CR-Falcon Laser 10W)

#### Flux Oak Wood 3mm

* Outline and switch holes: Cut 2 times with 4mm/s 100% power
* M2 holes: Cut 2 times with 4mm/s 100% power
* Kerf Switch-Holes: 0mm
* Kerf für Rand: +0.2mm

#### Acryl 3mm

* Kerf Switch-Holes: -0.15mm
* Kerf Rand: +0.2mm

#### For 3d printed  case and laser cut case

* top-foam-plate: 1mm thick, cut 15mm/s 90%
* bottom-foam-plate: 3mm thick, cut 12mm/s 90% 2 passes

### Measurements

#### With PCB as top-plate and 3mm acryl top middle plate

* Standoffs must be 6mm high, 3mm diameter
* Screw from bottom M2x6mm (6.8mm total)
* Screw from top M2x4mm (4.8mm total)

#### With acryl as top-plate and 2mm? acryl top middle plate

* Standoffs must be 6mm
* Screw from bottom and bottom M2x6mm (6.8mm total)
