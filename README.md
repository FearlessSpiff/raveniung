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

or for building including the left case:

```bash
ergogen . && npx @jscad/cli@1 output/cases/LeftCase.jscad -of stla
```

### TODO

* Add and route I2C FPC connector
* Verify change switch on/off direction -> Check on printed PCB
* Design new case for Azoteq TPS65
* Finish and measur 6pin ffc connector

## Notes

* mirror right case!

### Laser cutting (CR-Falcon Laser 10W)

#### Flux Oak Wood 3mm

* Outline and switch holes: Cut 2 times with 5mm/s 90% power
* M2 holes: Cut 2 times with 5mm/s 100% power

### Measurements

#### With PCB as top-plate and 3mm acryl top middle plate

* Standoffs must be 6mm high, 3mm diameter
* Screw from bottom M2x6mm (6.8mm total)
* Screw from top M2x4mm (4.8mm total)

#### With acryl as top-plate and 2mm? acryl top middle plate

* Standoffs must be 6mm
* Screw from bottom and bottom M2x6mm (6.8mm total)
