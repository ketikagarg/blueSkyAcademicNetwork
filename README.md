# blueSkyAcademicNetwork

#### Author: KG

#### 30 Nov 2024

<!-- Last updated: # 06 Dec 2024 -->

Last updated: 16 Mar 2025

This repository stores an interactive network file of the academic starter packs. The data here has been pulled from https://blueskydirectory.com/starter-packs/all and from bluesky's open data, with the help of blueksy developer APIs (https://docs.bsky.app/).

Each node is an academic starter pack. Connections (or edges) between any two given packs are based on the number of shared members between them. Community detection is done using louvain method, which seems to work pretty well so far, imo.

Gender detection: To classify, I use the pronouns used by members, and if none are present, I use Gender API in Python.

[Network Viz](https://ketikagarg.github.io/blueSkyAcademicNetwork/network2.html)

These do not cover all the academic starter packs in the interest of easier data handling. Main filter applied was the presence of at least 4 members between packs to register an edge between them (to remove spurious connections). There are currently ~1300 packs included.

<!-- If you are curious to see around 3500 nodes in a network with the filter that 1 shared member is sufficient: [whole Network](https://ketikagarg.github.io/blueSkyAcademicNetwork/wholeNetwork.html) -->

Other filtering criteria:

- I remove members that are not people. Not always perfect. I use NLP for this.
- I remove packs that are less than 5 in size.
- I use NLP to detect whether a pack is related to research or not. I keep packs only beyond a certain threshold.
- I remove packs that refer to a particular person rather than a topic. For example, X's starter pack.

I will continue updating the network as starter packs grow.

Contact me at [kgarg@caltech.edu](mailto:kgarg@caltech.edu) for more details or if interested in exploring this data together!

Enjoy!
