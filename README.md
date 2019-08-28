# Nokia-SR-PCE
Nokia PCE Segment Routing testing
Included here are the Test configurations for PCE testing with Nokia SROS as well as the Topology and Eve-NG Lab XML File. This repo consists of a 6 Router Lab utilizing Nokia SROS 19 for testing of PCE and PCEP with external Segment routing controllers. This should provide enough configuration to test PCE and PCEP against the Nokia SR series vSIMs.

### Files and such

1. flatten.sh - A script that takes the SROS configuration and converts it to a paste-able, flattened format. Requires https://github.com/door7302/transcode-sros
2. files named .flat.txt - flattened filed produced by the above script
3. vsr* Nokia SROS configurations as stored in the flash. Usable in the "startup configuration" for Eve-NG
4. Nokia PCE Lab.unl - the Eve-NG XML file that is the lab

### Diagrams and physical layout

The Physical layout of this test environment is detailed in this diagram. There are two virtualization platforms - one a dedicated EVE-NG bare metal server with significant horsepower. The second is a VMWare cluster that runs the Nokia NFM-P, NRC-P, and NRC in a redundant manner. VSR-NRC and NRCP and NFMP will be added soon.
![Physical lab Topology](https://github.com/buraglio/Nokia-SR-PCE/blob/master/netlab-virtlab-physical-pub.png?raw=true "Physical Lab Topology")

The logical topology inside of eve-ng looks roughly like this.  
![Virtual Router Topology](https://github.com/buraglio/Nokia-SR-PCE/blob/master/PCE%20Eve-NG%20Test%20Topology.png?raw=true "Virtual Router Topology")
