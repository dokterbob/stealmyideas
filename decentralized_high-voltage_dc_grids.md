# Decentralized High-Voltage DC grids
Current electricity grids are based on technology invented by Nikola Tesla, which was only ever meant as an intermediate stage before realizing a global and freely acessible energy distribution system using resonances on the earth's crest. However, due to a disease typically referred to as capitalism, his dreams were never realized and, in fact, are further from being realized then ever imagined.

Moreover, with our currently knowledge of biological systems and their electrical properties, having the whole earth continually enveloped in a very strong electromagnetic field seems like a potentially disastrous plan.

Rather than furthering the excellent work of Nikola Tesla, it makes sense to try and move forward towards a sustainable society in a way that allows 'legacy' systems to coincide with its successors, allowing for free and open competition and forcing any new systems to compete economically as well as in sustainability.

One such method would be to design a fully decentralized electrical system based on higher (~400V) DC voltages, where focus is put on local or regional energy self-sufficiency: instead of optimizing for low transport losses, optimization is done to maximize local resilience, stability and diversity. The idea is to fully decentralize the storage, production and distribution of energy such that any participant in the electrical grid performs an active role and, by material necessity, has a real but naturally limited power over the implementation of the system. In other words; participants are economically bound to cooperative participation.

However, on a larger scale, local systems *can* and should be connected to other systems, whether 'legacy' AC systems or other autonomous cooperatives. This allows for open competition between 'legacy' systems and decentralized alternatives, allowing for a smooth transition and consumer choice. Moreover, it allows for selling and buying of energy and storage capacity on larger scales - enabling the inclusion of necessarily larger-scale production and storage methods such as existing hydroelectrical projects.

More technically, the system would consist of high and lower voltage components, together with decentrally organized algoritms that govern the storage, transport, generation and consumption of electrical energy. The lower voltage can be different per connected unit, but will typically be a safe, common, low voltage such as 48V. The higher voltage end will be varying voltage between 360 and 400V; the voltage itself, together with internet-based data-exchange, will be leading in determining the behaviour of nodes in the network.

## Components
### DC/DC Convertion modules
#### AC Turbines (source)
* 2-phase 0-400 VAC -> 400 VDC
* 3-phase 0-400 VAC -> 400 VDC

#### Turbine/motor combination (source/sink)
* 2-phase AC <-> 360-400 VDC
* 3-phase AC <-> 360-400 VDC

#### Photovoltaic (source)
* LV DC -> 400 VDC (MPPT)

#### DC sinks
* 360-400 VDC -> ~48 VDC (in-house voltage, high-tolerance/high-power sinks)
* ~48 VDC -> 5-24 VDC (digital household devices)

#### AC sinks (legacy devices)
* 360-400 VDC -> 230 VAC 
* 360-400 VDC -> 380 VAC

#### Battery storage (source/sink)
* LV DC <-> 360-380 VDC

#### Bus interconnect (flow to/from other nodes/households)
* 360-400 VDC <-> 360-400 VDC

### Energy router
Every point were different sources or sinks interconnect are equipped with a generic power router, essentially a central bus controller for the 360-400 VDC bus. The power router controls individual DC/DC convertor modules, is internet-connected and performs decentralized management of the grid together with peer routers.

#### Communication
1. Bus voltage changes (360-380 VDC for sinks, 380-400 VDC for sources)
2. IPv6 over PLC/ZigBee/Wifi for accounting and high-level/long-term supply/demand management

#### Security
1. Centrally *signed* firmware updates with rollback
2. Communication fully encrypted using existing, battle-tested, protocols
4. Microcontrollers for power conversion hermetically seperated from system control logic 
