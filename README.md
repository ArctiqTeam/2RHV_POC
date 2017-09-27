# 2RHV_POC
a POC build of 2 RHV/oVirt (v4.1) servers, all orchestrated by Ansible

_(Designed to run in Ansible 'Core'/ open-source or Red Hat supported Ansible Engine)_

Files:
* bld-glstr.yml	-- to build a gluster pool.
* bld-rhv.yml	-- to build a RHV/oVirt self-hosted hypervisor
* hosted-engine-answer-file.conf.j2 -- ansible template for an answer file to deploy the hosted-engine.
* hosts -- ansible inventory file
* order-of-events.md -- steps taken.
* DNS config templates coming soon.

NOTE! The storage layer needs to be built before this hosted-engine will deploy!
 * for this we have: [bld-glstr.yml](https://github.com/ArctiqTeam/2RHV_POC/blob/master/bld-glstr.yml)

NOTE! A REAL DNS server must be available to the node doing the install!
 * for this, I've added: [setup-dns.yml](https://github.com/ArctiqTeam/2RHV_POC/blob/master/setup-dns.yml)
