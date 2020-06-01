# Sumo-Traffic-Simulations
This repository was clone from https://github.com/dyanni3/Traffic-Simulations/tree/master/grid-lights-lanes-github

Simulating dynamics on a 5x5 Manhattan-like grid using the SUMO package.

```bash
$ netgenerate --grid --grid.number=3 --grid.length=100 --output-file=grid.net.xml
$ python randomTrips.py -n grid.net.xml -e 600 -o grid.trips.xml
$ duarouter --net-file grid.net.xml --trip-files grid.trips.xml -o grid.rou.xml

$ sumo-gui -c grid.sumocfg --no-internal-links
```
