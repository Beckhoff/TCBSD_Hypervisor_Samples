# Basic VM script

`samplevm` is intended as minimalistic example to demonstrate the basic building blocks for scripting a bhyve based virtual machine configuration.

## Usage

To install the script on the system run:

```
doas make
```

Afterwards the `samplevm` can be started via:

```
doas samplevm
```

The virtual machine will boot into the UEFI Shell environment which is printed to the console because the machines `COM1` port is redirected to the standard input and output streams.

```
UEFI Interactive Shell v2.2
EDK II
UEFI v2.70 (BHYVE, 0x00010000)
map: No mapping found.
Press ESC in 1 seconds to skip startup.nsh or any other key to continue.
Shell>
```

You can return to the console by shuting down the VM via the UEFI shell command `reset -s`.

```
UEFI Interactive Shell v2.2
EDK II
UEFI v2.70 (BHYVE, 0x00010000)
map: No mapping found.
Press ESC in 1 seconds to skip startup.nsh or any other key to continue.
Shell> reset -s
```
