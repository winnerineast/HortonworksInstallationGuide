# HortonworksInstallationGuide
## background
### I were assigned to design a big data systems in multiple servers, so I decided to test my design in my two laptop first with hortonworks data platform.

## Environment
- one Macbook Pro (CPU i7,Memory 16GB, MacOS Sierra), abbr. MBP
- one Surface Pro3(CPU i5,Memory 8GB, Windows 8.1), abbr. SP3

## Big Data System Deployment Goal
- Phase1: setup Hortonworks HDP sandbox in both MBP and SP3 and the user could access them from either MBP or SP3 in both hosts and VMs.
- Phase2: configure MBP as Ambari master and SP3 as slave and the user could access them from either MBP or SP3 in both hosts and VMs.
- Phase3: shift invidvidual components between MBP and SP3 and the user could access them from either MBP or SP3 in both hosts and VMs.
- Phase4: shift all deployments into Docker.

## Installation Steps
### 1. Prepare OS in MBP
- 1.1 Reboot the system and press command key and R at the same time when the system bootup to enter rescure model.
- 1.2 Erase all partions and re-install MacOS Sierra.
- 1.3 Use all default configuration to setup MacOS Sierra.
### 2. Prepare OS in SP3
- 2.1 Reboot the system and press power key and volumn up key at the same time when the system boot up to enter rescure model.
- 2.2 Choose restore factory model.
- 2.3 Use all default configuration to setup Windows 8.1.
### 3. Phase1 setup
- 3.1 Download and install [virtualbox](https://www.virtualbox.org/wiki/Downloads)for both Windows and OS X hosts.
- 3.2 Download and install [Hortonworks HDP](http://hortonworks.com/downloads/)
- 3.3 Test Hortonworks sandbox to be running successfully in both MBP and SP3.
- 3.4 Setup bridge network card as second virtual network adapter card in both HDP VMs and keep the first virtual network adapter card as NAT without any change.
