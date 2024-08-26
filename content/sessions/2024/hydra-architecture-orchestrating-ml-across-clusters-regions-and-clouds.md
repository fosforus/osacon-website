---
title: "Hydra Architecture: Orchestrating ML across clusters, regions, and clouds"
slug: hydra-architecture-orchestrating-ml-across-clusters-regions-and-clouds
speakers:
 - Donny Greenberg
topics:
 - Infrastructure
room: 
time_start: 2024-11-19T09:00:00-04:00
time_end: 2024-11-19T09:25:00-04:00
---

Increasingly, ML teams must satisfy requirements for executing workflows across multiple Kubernetes clusters, regions, or clouds. Challenges include constrained GPU availability within a single cloud, cloud credits or commitments across multiple providers, or strict data residency requirements. Traditional methods for replicating workflows across environments are both resource-intensive and operationally cumbersome. 
 
 
 
 In this talk, we propose a Hydra architecture, a novel approach where applications are deployed to a single cluster but can selectively take advantage of others. Management and orchestration happens in a single cluster, but execution flows flexibly through arbitrary remote compute. To accomplish this, we will articulate an open source approach that allows standard Python programs to be dispatched to any compute resource without repackaging multiple deployments for each compute locale or otherwise imposing restrictions. By unbundling orchestration and execution, ML platforms teams can now provide their fleet of compute to the practitioners in a single abstract layer.