# blueSkyAcademicNetwork

#### Author: KG

#### 30 Nov 2024

This repository stores an interactive network file of the academic starter packs. The data here has been pulled from https://blueskydirectory.com/starter-packs/all and from bluesky's open data, with the help of blueksy developer APIs (https://docs.bsky.app/).

Each node is an academic starter pack. Connections (or edges) between any two given packs are based on the number of shared members between them. Community detection is done using louvain method, which seems to work pretty well so far, imo. But I can explore other methods, too.

There are two network files available for visualization. Play around to see which one you prefer:

- [Network 1](https://ketikagarg.github.io/blueSkyAcademicNetwork/network1.html)
- [Network 2](https://ketikagarg.github.io/blueSkyAcademicNetwork/network2.html) this is better!

These do not cover all the academic starter packs in the interest of easier data handling. Main filter applied was the presence of at least 3 members between packs to register an edge between them (to remove spurious connections). There are currently ~1000 packs included. If you are curious to see around 2000 nodes in an network without the filter: [whole Network](https://ketikagarg.github.io/blueSkyAcademicNetwork/wholeNetwork.html)

I will continue updating the network as starter packs grow.

Contact me at [kgarg@caltech.edu](mailto:kgarg@caltech.edu) for more details or if interested in exploring this data together!

Enjoy!
