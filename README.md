# Mastering-Service-Mesh-Architecture

## Build Environment

### Using Docker Desktop on Windows

A single node Kubernetes environment using Docker Windows Container can be build on Windows 10 machine (or laptop) for the purpose of this book. Refer to [https://docs.docker.com/v17.09/docker-for-windows/install/](https://docs.docker.com/v17.09/docker-for-windows/install/) using Edge channel - which provides a convenient method to use single node Kubernetes on Windows 10. Install using [https://www.docker.com/products/docker-desktop](https://www.docker.com/products/docker-desktop).

In Windows 10, Hyper-V needs to be turned on to run Docker for Windows but this will not allow VMWare to run virtualization. 

Use Script [scripts/enable.cmd](scripts/enable.cmd) to turn on Hyper-V for `Docker for Windows Desktop` and [scripts/disable.cmd](scripts/disable.cmd) to turn-off Hyper-V if VMware virtualization is to be used. This will require reboot. The script `enable.cmd/disable.cmd` runs PowerShell script [scripts/hyperv.ps1](scripts/hyperv.ps1) to turn-on or turn-off Hyper-V.

### Using Docker Desktop Edge on Mac

Docker Desktop for Mac provides a single node Kubernetes environment - which is good for development purposes. Start using [https://www.docker.com/products/docker-desktop](https://www.docker.com/products/docker-desktop)

### Using IBM Cloud Private on Linux VMs

Refer to repo [https://github.com/servicemeshistio/icp](https://github.com/servicemeshistio/icp) - if you want to build an enterprise like multi-node Kubernetes environment. IBM Cloud Private Community edition is free. You can build a robust 3 node cluster on your laptop if you have 32 GB RAM and VMware Workstation. Consult the repo.
