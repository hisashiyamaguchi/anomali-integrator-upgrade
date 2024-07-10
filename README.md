# Anomali Integrator quick upgrade guide.
The objective of the RM is to show how you can upgrade your on-premise Anomali Integrator.

## Prerequisite
- SSH access to your Anomali Integrator.
- You have already downloaded Integrator tar.gz, and upload it to your Integrator instance.

## Upgrade
Login your Integrator instance, and check the status is running.

```console
$ /opt/bin/integrator status
Integrator is running (PID:30308)
```
<br>

Unzip and untar the donwloaded Integrator, and execute the installer as root.
```console
$ gunzip xxxx.tar.gz
$ tar xvf xxxx.tar4
$ sudo ./integrator_xxxx_linux64.2.bin
```

Specify the current install directry. **Do NOT specify the different directory of the current install directory. The path should be exactly the same as the current install directory.**
```console
Verifying archive integrity... All good.
Uncompressing Anomali Integrator.................................................................................................
Enter Anomali Integrator installation directory: ^CSignal caught, cleaning up
sudo ./integrator_8.4.1_linux64.2.bin
[sudo] password for aintegrator:
Verifying archive integrity... All good.
Uncompressing Anomali Integrator.................................................................................................
Enter Anomali Integrator installation directory: /opt
Old version found, Do you want to upgrade it? [y/n] y
Upgrading...
Checking if Integrator currently has a sync in progress
```


## Issue Reporting
If you have found a bug or if you have updates request, please report them at this repository issues section.