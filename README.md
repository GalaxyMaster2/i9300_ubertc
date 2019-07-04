# i9300_ubertc

Modified scripts for building UBER toolchains with Cortex A9 optimizations and using slightly newer binutils

# How to use:

1. Initialize and sync an UBER toolchain repo as described here: https://github.com/UBERTC/uber-manifest
2. Download all the files from the `scripts` directory of this repository and place them in the `scripts` directory of your local UBER toolchain repo. Overwrite any existing scripts if necessary.
3. Execute one of the scripts to build the corresponding toolchain. The scripts of interest are:

* `./arm-cortex_a9-eabi-4.9`
* `./arm-cortex_a9-eabi-5.x`
* `./arm-cortex_a9-eabi-6.x`
* `./arm-cortex_a9-eabi-7.x`
* `./arm-cortex_a9-eabi-8.x`
* `./arm-cortex_a9-linux-androideabi-4.9`
* `./arm-cortex_a9-linux-androideabi-5.x`
* `./arm-cortex_a9-linux-androideabi-6.x`
* `./arm-cortex_a9-linux-androideabi-7.x`
* `./arm-cortex_a9-linux-androideabi-8.x`

as well as the same ones without `cortex_a9` in the name. The scripts with only `eabi` in the name are kernel toolchains, the ones with `linux-androideabi` in the name are for the rest of the rom. The number at the end is the GCC version number. The scripts with `cortex_a9` in the name build toolchains with specific Cortex A9 optimizations.
