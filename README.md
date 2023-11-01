# PTP
## Introduction
This repository basically consists of an ansible directory structure that contains an ansible role that would deploy the linuxptp software package into FABRIC VMs in the experimenter's FABRIC slice. A sample playbook [playbook_fabric_experiment_ptp.yml](ansible/playbook_fabric_experiment_ptp.yml) is also included that demonstrates its use in an ansible playbook.

## PTP Support in FABRIC Experiments
FABRIC provisions virtual machines that are KVM based VMs for user experiment nodes upon request by FABRIC users. Any modern Linux operating system (using a modern kernel > 3.x ) use support a device called ptp_kvm that essentially emulates a PTP clock device. The host system KVM provides this ptp_kvm device located inside the virtual machine its system time

![](images/timing.png)