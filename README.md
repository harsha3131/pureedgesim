<img width= "20%" src="https://user-images.githubusercontent.com/46229052/196671093-21ba3438-719d-4dd4-ad79-bfddd1395663.png" align="right" />

# PureEdgeSim

PureEdgeSim: A simulation framework for performance evaluation of cloud, edge and mist computing environments

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![Build Status](https://app.travis-ci.com/harshajoshi3103/PureEdgeSim.svg?branch=master)](https://app.travis-ci.com/harshajoshi3103/PureEdgeSim) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/7bcee5c75c3741b5923e0158c6e79b37)](https://www.codacy.com/gh/harshajoshi3103/PureEdgeSim/dashboard) [![Maven Central](https://img.shields.io/maven-central/v/com.mechalikh/pureedgesim.svg?label=Maven%20Central)](https://search.maven.org/search?q=g:%22com.mechalikh%22%20AND%20a:%22pureedgesim%22) [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/7bcee5c75c3741b5923e0158c6e79b37)](https://www.codacy.com/gh/harshajoshi3103/PureEdgeSim/dashboard)


![image](https://user-images.githubusercontent.com/46229052/196698541-569de31b-0df8-470b-907c-02ba5eb5015f.png)

## Please Cite It As:

Mechalikh, C., Taktak, H., & Moussa, F. (2021). PureEdgeSim: A simulation framework for performance evaluation of cloud, edge and mist computing environments. Computer Science and Information Systems, 18(1), 43-66.

Mechalikh, C., Safavifar, Z., & Golpayegani, F. (2025). Quality matters: A comprehensive comparative study of edge computing simulators. Simulation Modelling Practice and Theory, 138, 103042.

Bibtex:

```js
@article{mechalikh2021pureedgesim,
  title={PureEdgeSim: A simulation framework for performance evaluation of cloud, edge and mist computing environments},
  author={Mechalikh, Charafeddine and Taktak, Hajer and Moussa, Faouzi},
  journal={Computer Science and Information Systems},
  volume={18}
  number={1},
  pages={43--66},
  year={2021}
}



@article{mechalikh2025quality,
  title={Quality matters: A comprehensive comparative study of edge computing simulators},
  author={Mechalikh, Charafeddine and Safavifar, Zahra and Golpayegani, Fatemeh and others},
  journal={Simulation Modelling Practice and Theory},
  volume={138},
  pages={103042},
  year={2025},
  publisher={Elsevier}
}
```

## Version 5.1 Changelog (October 18th 2022)

<details>
<summary>"Click to expand"</summary>

*   Updated the energy model with the ability to set an initial battery level for generated devices, either programmatically or via the xml file. 

*   Now users can extend the simulation manager to change its behavior, and easily integrate it in the simulation.

*   Users can now easily integrate a custom task class.

*   All entities are now notified at the end of the simulation through onSimulationEnd() method.

*   Failure Model: now tasks can fail due to insufficient resources: RAM, STORAGE, CPU Cores.

*   Disabled some unnecessary network links events/loops for better performance.

*   Now tasks can be scheduled in batches instead of being scheduled all at once at the beginning of the simulation (hence, decreasing the number of events and therefore, faster simulations and less memory usage).

*   Removed unnecessary loops when orchestrating tasks (e.g., no need to browse through edge devices when the cloud only architecture is used, etc.) 

*   Overall version 5.1 can be 30 times faster and supports up to 8 times the number of tasks compared to previous version 5.0 (see figure below).

*   Improved extensibility: Users can now easily incorporate a custom task class, custom simulation manager, as well as a custom topology creator.

*   Now applications placement decisions are done after each failure (default behavior, can be changed by extending the DefaultSimulationManager and DefaultOrchestrator classes).

*   Reduced duplication and improved code quality.

*   Other fixes..

<p align="center">
  <img  width="500" src="https://user-images.githubusercontent.com/46229052/196478109-29442658-19c1-498e-9c0e-593780e12f44.png">
</p>

<p align="center">A comparison of simulation duration between the previous version 5.0 and the latest version 5.1</p>

</details>

<br></br>
![image](https://user-images.githubusercontent.com/46229052/196704278-4d04778b-1a9e-46da-9ae2-18e6a7a1bae5.png)
<a id="overview"></a>

<img width="20%" src="https://user-images.githubusercontent.com/46229052/196671599-c2c33b14-be0b-4f7a-92b2-533978afb029.png" align="right" />
<p align="justify">
PureEdgeSim is a simulation framework that enables to study Internet of Things on a large scale, as a 
distributed, dynamic, and highly heterogeneous infrastructure, as well as the applications 
that run on these things. It features realistic infrastructure models, allowing research on the edge-to-cloud continuum to be conducted. It
encompasses all layers of edge computing modeling and simulation.
It features a modular design in which each module addresses a particular aspect of the 
simulation. The Datacenters Manager module, for example, is concerned with the creation 
of data centers, servers, as well as end devices and their heterogeneity. Their geo-distribution 
and mobility, however, are handled by the Location Manager module. Similarly, the 
Network Module is in charge of bandwidth allocation and data transfer. </p>


<!-- REST OF README CONTENT -->

## Maintainer

This project is currently maintained by Sri Harsha Joshi.  Original work by Charafeddine Mechalikh is gratefully acknowledged.

For any inquiries, please contact:

* Email: harshajoshi3103@gmail.com


<img width= "20%" src="https://user-images.githubusercontent.com/46229052/196670788-1b7ff2fc-4958-4645-8254-0ea516e035bc.png" align="left" />
