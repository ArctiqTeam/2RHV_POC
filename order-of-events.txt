# RHVBuilder README.md

RHV builder

step 1..

- install RHEL/CENTOS on hosts that will be hypervisors
- decide how many hosts will be self-hosted engine installs
- propagate Ansible user SSH keys to hosts that will be hypervisors.

step 2..

- install necessary packages for RHV/oVirt
- for the self-hosted engine hosts, install the relevant self-hosted engine packages

step 3..

- prepare an answers file for the RHV/oVirt setup script to consume
- pre-download the self-hosted engine image rpm

step 4..

- decide on storage layout, and prepare storage before setup continues
- verify storage before continuing
- ensure isolated 54GB export is available per host for each engine

step 5..

- provide storage and network and various settings into your answer file.
- deploy via the setup script with the answer file on each destined hypervisor.

step 6..

- WAIT FOR the engine to self-initialize and read the storage it was given from the answer file

step 7..

- initialize the data-center from the web-GUI by adding and initializing the appropriate ISO and storage mounts
- WAIT FOR the engine to initialize the storage your just added.

step 8..

- propagate ansible keys to engines.
