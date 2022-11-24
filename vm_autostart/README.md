# VM autostart sample

This folder includes files to demonstrate a basic example how to connect a scripted VM configuration with the rc.d framework so that a VM can be run as a service on system startup.

## Install sample

Within this directory run:

```
doas make
```
to install the sample on the system.

Afterwards the `samplevm` script can be controlled via the `service` command.

## Controlling the VM service

To enable or disable the `samplevm` as a system service run either:

```
doas service samplevm enable
```

or

```
doas service samplevm disable
```

If `samplevm` is enabled in `/etc/rc.conf` the VM can be manually started via:

```
doas service samplevm start
```

The state of the VM service can be quired via:

```
doas service samplevm status
```

In this sample the VM can be accessed via a VNC client on TCP port `5900`.

To stop the VM via the `service` command run:

```
doas service samplevm start
```
