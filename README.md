# Kubernetes Hands-On

## Prerequisites
Windows, Linux, or Mac workstation with minimum of 2 CPU cores and 8GB of RAM
Software:
  - VirtualBox (https://www.virtualbox.org)
  - Vagrant (https://www.vagrantup.com)
  - Git (https://git-scm.com/downloads)

_(Make sure latest versions are installed)_


## Setup Environment
Clone this repository and bring up the VMs that we'll use for our Kubernetes cluster

```
git clone https://github.com/stoyansbg/kubernetes-hands-on.git
cd kubernetes-hands-on
vagrant up
```

**Note:** Mac users, if you encounter an error like this:
```
There was an error while executing `VBoxManage`, a CLI used by Vagrant
for controlling VirtualBox. The command and stderr is shown below.

Command: ["hostonlyif", "create"]

Stderr: 0%...
Progress state: NS_ERROR_FAILURE
VBoxManage: error: Failed to create the host-only adapter
VBoxManage: error: VBoxNetAdpCtl: Error while adding new interface: failed to open /dev/vboxnetctl: No such file or directory
VBoxManage: error: Details: code NS_ERROR_FAILURE (0x80004005), component HostNetworkInterfaceWrap, interface IHostNetworkInterface
VBoxManage: error: Context: "RTEXITCODE handleCreate(HandlerArg *)" at line 95 of file VBoxManageHostonly.cpp
```

, go to **Settings -> Security & Privacy -> General -> System software from developer "Oracle America, Inc"...** and click on the **[Allow]** button.  You will need to restart for the changes to take effect.
