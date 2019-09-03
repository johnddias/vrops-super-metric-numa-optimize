# vRealize Operations Super Metric - Optimize VM CPU for NUMA
This sample includes two Super Metrics which are based on the VMware Fling "Virtual Machine Compute Optimizer" which provides a report of VMs with recommended CPU socket and core configuraiton based on the VM resource allocation for CPU and memory and the ESXi host configuration.

To use these samples, import using Administration > Configuration > Super Metrics and assign to VM object types and then enable in policy (you can also use Super Metric preview if you prefer not to enable in policy).

The sample uses two super metrics, one to calculate the optimal number of cores per socket and the other to calculate the optimal number of sockets.  They are the same with some minor additional calculation doen for the optimal number of cores per socket.

This was created using vRealize Operations 7.5.  Here's a sample of the output in a view:
![NUMA Report Sample View](https://github.com/johnddias/vrops-super-metric-numa-optimize/blob/master/NUMA%20View.JPG)

