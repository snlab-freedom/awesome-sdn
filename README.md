# Awesome - Software Defined Networking

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) [![Build Status](https://travis-ci.org/snlab-freedom/awesome-sdn.svg?branch=master)](https://travis-ci.org/snlab-freedom/awesome-sdn)

A curated list of awesome SDN (Software Defined Networking) papers, projects and communities. Inspired by [awesome-go](https://github.com/avelino/awesome-go) and [awesome-deep-learning-papers](https://github.com/terryum/awesome-deep-learning-papers).

<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-generate-toc again -->
**Table of Contents**

- [Awesome - Software Defined Networking](#awesome---software-defined-networking)
    - [Background](#background)
    - [Software Projects](#software-projects)
        - [Distributed Network OS](#distributed-network-os)
        - [Controller](#controller)
        - [Software Switch](#software-switch)
        - [Network Devices Support](#network-devices-support)
        - [Protocol](#protocol)
        - [SDN Application](#sdn-application)
        - [Network Programming Language](#network-programming-language)
        - [Network Virtualization](#network-virtualization)
        - [Library](#library)
        - [Simulator / Emulator](#simulator--emulator)
        - [NetDevOp](#netdevop)
        - [Network Monitor / Analysis](#network-monitor--analysis)
        - [Test Tool](#test-tool)
        - [Orchestrator](#orchestrator)
        - [Misc](#misc)
    - [Hardwares](#hardwares)
        - [OpenFlow Switch](#openflow-switch)
        - [NetFPGA](#netfpga)
        - [Chips](#chips)
    - [Research Papers](#research-papers)
        - [Additional Research Papers](#additional-research-papers)
    - [Tutorials](#tutorials)
        - [OpenDaylight](#opendaylight)
        - [ONOS](#onos)
    - [Courses](#courses)
    - [Communities](#communities)
        - [Organization](#organization)
        - [Social Forum / BBS](#social-forum--bbs)
        - [Q & A](#q--a)
    - [Acknowledgement](#acknowledgement)

<!-- markdown-toc end -->

## Background

Before this list, there exist other lists to summarize the resources about SDN, such as [Google SDN Reading List], [ONF Recommended SDN Reading List] and [Awesome SDN from sdnds-tw]. But these lists only focus on one aspect of the *classic* research papers, *popular* opensource projects and well-known communities. In my opinion, a comprehensive list about all of the aspects I just mentioned is necessary. Both beginners and professional people will benefit from it.

## Software Projects

The initial version is forked from [SDNDS-TW][Awesome SDN from sdnds-tw] but re-organized. Thanks again!

### Distributed Network OS

- [ONOS](http://onosproject.org) - Open Network Operating System.
- [OpenDaylight](https://www.opendaylight.org) - OpenDaylight Platform

### Controller

- [NOX](https://github.com/noxrepo/nox) - An open source development platform for C++-based software-defined networking (*SDN*) control applications.
- [NodeFlow](https://github.com/gaberger/NodeFLow) - An OpenFlow Controller Node Style.
- [POX](https://github.com/noxrepo/pox) - A networking software platform written in Python
- [Ryu](https://osrg.github.io/ryu) - A component-based software defined networking framework.
- [Floodlight](https://github.com/floodlight/floodlight) - A java-based openflow controller.
- [Vyatta](https://github.com/BRCDcomm/BVC/) - The first commercial Controller built directly from OpenDaylight.
- [OpenContrail](http://www.opencontrail.org/) - A SDN project that utilizes SDN & NFV and provides all the necessary components for network virtualization.
- [IRIS](http://openiris.etri.re.kr/) - A Resursive SDN Openflow Controller created by SDN Research Section, ETRI.
- [Open MUL](http://www.openmul.org/openmul-controller.html) - A lightweight SDN/Openflow controller written almost entirely in C from scratch.
- [OESS](https://github.com/globalnoc/oess) - The Open Exchange Software Suite to configure and control OpenFlow Enabled switches.
- [Beehive Network Controller](https://github.com/kandoo/beehive-netctrl) - A distributed SDN controller built on top of Beehive. It supports OpenFlow but can be easily extended for other southbound protocols.
- [Ravel](https://github.com/ravel-net/ravel) - A software-defined networking (SDN) controller that uses a standard SQL database to represent the network.
- [Trema](https://trema.github.io/trema/) - A full-stack, easy-to-use framework for developing OpenFlow controllers in Ruby and C.

### Software Switch

- [OpenvSwtich](http://openvswitch.org/) - Open vSwitch is a production quality, multilayer virtual switch.
- [Indigo](https://github.com/floodlight/indigo) - Indigo is an open source project aimed at enabling support for OpenFlow on physical and hypervisor switches.
- [CPqD](https://github.com/CPqD/ofsoftswitch13)- An OpenFlow 1.3 compatible user-space software switch implementation
- [Lagopus](https://lagopus.github.io) - A high-performance software OpenFlow 1.3 switch.
- [LINC-Switch](https://github.com/FlowForwarding/LINC-Switch) - A pure OpenFlow software switch written in Erlang
- [snabbswitch](https://github.com/SnabbCo/snabbswitch) - An open source virtualized Ethernet networking stack.

### Network Devices Support

- [PicOS](http://www.pica8.com/products/picos) - A SDN OS for white box switches Layer-2/3 feature set with support for OpenFlow, OVSDB, and other protocols.
- [OpenNetworkLinux](https://opennetlinux.org) - A Linux distribution for "bare metal" switches, that is, network forwarding devices built from commodity components.
- [OpenSwitch](http://www.openswitch.net) - A linux network oerating system from Hewlett-Packard.

### Protocol

- [OpenFlow](https://www.opennetworking.org/sdn-resources/openflow) - A communications protocol that gives access to the forwarding plane of a network switch or router over the network.
- [OF-Config](https://www.opennetworking.org/technical-communities/areas/specification/1928-of-config) - OpenFlow Management and Configuration Protocol
- [OVSDB](https://tools.ietf.org/html/rfc7047) - A communication protocol which used to manage the OpenvSwitch database.
- [POF](http://www.poforwarding.org/) - Protocol Oblivious Forwarding

### SDN Application

TBD

### Network Programming Language

- [P4](http://p4.org/) - A declarative language for expressing how packets are processed by the pipeline of a network forwarding element such as a switch, NIC, router or network function appliance.
- [Frenetic](https://github.com/frenetic-lang/frenetic) - The Frenetic Programming Language and Runtime System
- [Pyretic](http://www.frenetic-lang.org/pyretic/) - Pyretic is one member of the Frenetic family of SDN programming languages.
- [NEMO](https://wiki.onosproject.org/display/ONOS/NEMO+Language) - A domain specific language (DSL) based on abstraction of network models and conclusion of operation patterns.

### Network Virtualization

- [FlowVisor](https://github.com/opennetworkinglab/flowvisor) - An OpenFlow controller that acts as a hypervisor/proxy between a switch and multiple controllers. Can slice multiple switches in parallel, effectively slicing a network.
- [OpenVirtex](https://github.com/opennetworkinglab/OpenVirteX) - A network hypervisor that can create multiple virtual and programmable networks on top of a single physical infrastructure.

### Library

- [loxigen](https://github.com/floodlight/loxigen) - LoxiGen is a tool that generates OpenFlow protocol libraries for a number of languages.
- [openfaucet](https://github.com/rlenglet/openfaucet) - openfaucet is a pure Python implementation of the OpenFlow 1.0.0
protocol, based on Twisted.
- [oflib-node](https://github.com/TrafficLab/oflib-node) - Oflib-node is an OpenFlow protocol library for Node. It converts between OpenFlow wire protocol messages and Javascript objects.
- [OpenFlowJ](https://bitbucket.org/openflowj/openflowj) - A Java implementation of low-level OpenFlow packet marshalling/unmarshalling and IO operations.
- [nettle](http://haskell.cs.yale.edu/other-projects/nettle/) - A Haskell library for working with the OpenFlow protocol.
- [OCaml OpenFlow](https://github.com/frenetic-lang/ocaml-openflow) - A serialization and protocol library for OpenFlow.

### Simulator / Emulator

- [Mininet](http://mininet.org/) - An Instant Virtual Network on your Laptop (or other PC)
- [OpenNet](http://github.com/dlinknctu/opennet) - A simulator for software-defined wireless local area network
- [EstiNet](http://www.estinet.com/products.php?lv1=13&sn=13) - A world-renowned software tool for network planning
- [ns-3](https://www.nsnam.org/) - A discrete-event network simulator that supports openflow environment.

### NetDevOp

- [NetIDE](https://github.com/fp7-netide/Engine) - Enable Network App programs to be executed, systematically tested, and refined on a variety of concrete SDN platforms.

### Network Monitor / Analysis

- [PerfSonar](http://www.perfsonar.net/) - perfSONAR is a network measurement toolkit designed to provide federated coverage of paths, and help to establish end-to-end usage expectations.

### Test Tool

- [oftest](https://github.com/floodlight/oftest) - OpenFlow Testing Framework
- [STS](https://ucb-sts.github.com/sts/) - SDN Troubleshooting System, simulates network devices, allowing programmatically test cases generation.
- [nice-of](https://code.google.com/archive/p/nice-of/) - A tool to test OpenFlow controller application for the NOX controller platform.
- [OpenSDNCore](http://www.opensdncore.org/) - Virtualisation Testbed for NFV/SDN Environment.

### Orchestrator

- [OPEN-Orchestrator Project, Open-O](https://www.open-o.org)
- [Enhanced Controller Orchestration Management Policy, ECOMP](http://att.com/ecomp) - Operations management framework.

### Misc

- [Central Office Re-architected as a Datacenter, CORD](http://opencord.org) - Reference Implementation of a Service Delivery Platform that Provides Cloud Economies and Agility.
- [Open Source MANO Community, OSM](https://osm.etsi.org/welcome/)
- [ONIE](http://onie.org/) - ONIE enables a bare metal network switch ecosystem where end users have a choice among different network operating systems.

## Hardwares

### OpenFlow Switch

TBD

### NetFPGA

TBD

### Chips

TBD

## Research Papers

Please go to [ONF SDN Reading List][ONF Recommended SDN Reading List]. Thanks again to [ONF]!

### Additional Research Papers

Although ONF SDN Reading List has been very comprehensive, we may also find some other interesting papers. We will update this list into ONF SDN Reading List if necessary.

TBD

## Tutorials

### OpenDaylight

- [Controller Core Functionality Tutorials: Application Development Tutorial](https://wiki.opendaylight.org/view/Controller_Core_Functionality_Tutorials:Application_Development_Tutorial)

### ONOS

- [Official Tutorials Page](https://wiki.onosproject.org/display/ONOS/Tutorials)

## Courses

- [COMS E6998: Software Defined Networking](http://www.cs.columbia.edu/~lierranli/coms6998-10SDNFall2014/) by Li Erran Li, Fall 2014, Columbia University
- [CPSC 434/534: Topics in Networked Systems](http://zoo.cs.yale.edu/classes/cs434/cs434-2017-spring/schedule.shtml) by Y. Richard Yang, Spring 2017, Yale University

## Communities

### Organization

- [ONF] - Open Networking Foundation.
- [Open Source SDN](http://opensourcesdn.org/) - A collection of open source projects about SDN. Launched by ONF.
- [ON.Lab](http://onlab.us/)
- [SDxCentral](https://www.sdxcentral.com/)
- [SDNHub](http://sdnhub.org/)
- [IETF Software Defined Networking Research Group (sdnrg)](https://datatracker.ietf.org/rg/sdnrg/charter/)
- [SDNLAB](http://www.sdnlab.com/)

### Social Forum / BBS

TBD

### Q & A

- [OpenDaylight Q&A Forum](https://ask.opendaylight.org/questions/)

## Acknowledgement

Thanks to [Open Networking Foundation][ONF] for summarizing the awesome paper reading list.

Thanks to [SDNDS-TW](https://github.com/sdnds-tw) for drafting the awesome list of SDN software resources.

  [Google SDN Reading List]: https://sites.google.com/site/sdnreadinglist/
  [ONF Recommended SDN Reading List]: https://www.opennetworking.org/sdn-resources/sdn-reading-list
  [Awesome SDN from sdnds-tw]: https://github.com/sdnds-tw/awesome-sdn
  [ONF]: https://www.opennetworking.org/
