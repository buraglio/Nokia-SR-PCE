# Nokia-SR-PCE
Nokia PCE Segment Routing testing
Included here are the Test configurations for PCE testing with Nokia SROS as well as the Topology and Eve-NG Lab XML File. This repo consists of a 6 Router Lab utilizing Nokia SROS 19 for testing of PCE and PCEP with external Segment routing controllers

### Files and such

1. flatten.sh - A script that takes the SROS configuration and converts it to a paste-able, flattened format. Requires https://github.com/door7302/transcode-sros
2. files named .flat.txt - flattened filed produced by the above script
3. vsr* Nokia SROS configurations as stored in the flash. Usable in the "startup configuration" for Eve-NG
4. Nokia PCE Lab.unl - the Eve-NG XML file that is the lab

![Router Topology](https://github.com/buraglio/Nokia-SR-PCE/blob/master/PCE%20Eve-NG%20Test%20Topology.png?raw=true "Router Topology")
