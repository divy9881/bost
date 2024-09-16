# bost
BOST: Boice Object STore, a highly performant, reliable, multi-tiered, cost-efficient, distributed object store 

## Why Rust?
- Do not have to take care of memory management(unlike in C/C++) without involving an extravagant garbage collector(unlike Golang, Java)
- Cannot run into memory issues like double-free, use-after-free
- Catches most of the code-issues during compilation, and hence during runtime, very less last-minute surprises and fewer crashes
- Bindings available for most of the user-space libraries like io-uring, gRPC, etc
- Can achieve high-performance, which is a requirement of the system being implemented

## TODOs
- [] Optimal use of Storage tiers
- [] Highly scalable
    - [] Addition of new disks to the array
    - [] Addition of new nodes to the cluster
    - [] Decommisioning disks from the array
    - [] Decommisioning nodes from the cluster
- [] Kubernetes for orchestration
- [] Highly reliable and resilient
- [] High storage density for higher cost-efficiency
    - [] No fragmentation
    - [] Efficient Erasure Codes
- [] Object Versioning
- [] Incorporate gRPC for cross-node communication
- [] Support for I/O sub-systems
    - [] io-uring for newer kernerls
    - [] aio for older kernels
- [] RDMA support for bulk cross-node data transfers ?
- [] Disk format
    - [] Data
    - [] Metadata
- WORM ?
- [] Efficient and Performant Computations
    - [] Erase code computations
    - [] Bit-rot computations
- [] High throughput vs High latency ?
- [] Disaster Recovery -  Continuous replication
- [] Bit-rot protection
- [] Encryption
- [] Compression
- [] Global federation ?
- [] Self-healing objects ?
- [] Workload isolation mechanisms
- [] Authoriation
- [] Minimal use of locks
- [] Role-based work assignment
    - [] Node-level
    - [] Thread-level
- [] De-duplication ?
- [] AWS S3 compliant
- [] Special cases
    - [] Tiny objects (< 1 MB)
    - [] Huge objects (> 1 GB)
