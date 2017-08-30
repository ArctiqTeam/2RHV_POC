# 2RHV_POC
a POC build of 2 RHV servers, all orchestrated by Ansible


Files:
* bld-glstr.yml	-- to build a gluster pool.
* bld-rhv.yml	-- to build a RHV/oVirt self-hosted hypervisor
* hosted-engine-answer-file.conf.j2 -- ansible template for an answer file to deploy the hosted-engine.
* hosts -- ansible inventory file
* order-of-events.md -- steps taken.
* DNS config templates coming soon.

NOTE! The storage layer needs to be built before this hosted-engine will deploy!
NOTE! A REAL DNS server must be available to the node doing the install!
