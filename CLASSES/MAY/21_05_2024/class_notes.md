
# MAY, 21, 2024 - CLOUD COMPUTING CLASS

## CONTAINERS

Hypervisor make virtualization possible

- type 1: also know as bare metal
- type 2: the same as a virtual machine program, which means, hypervisor is running on another program.

advantages of using virtualization:

- better hardware utilization
- cheap hosting
- isolation
- portability

## cloud providers

Nowadays, we use providers to host our solutions.

For example, asking AWS for an instance with 2 CPUs, 4GB RAM each, 100GB storage and an operative system,
they are not renting us a physical server with required specifications.
Instead, they create a VM with all these spces using their well thought infrastructure.

### Do I really need VMs?

    There is no colored rainbow. Using VMs have also drawbacks:

    - They are heavy
    - They introduce overhead

    They might be the right solution for large scale, complex applications.

    - OS and software can be fine tuned
    - Heavy software and processing might require powerful VMNs

#### What if I have small applications?

    Only requisite is isolated environment.
    Should I rent 100s of VMs?


### Containers versus virtualization

    Isolated execution environment where one or many process can run

    `OS level Virtualization`

    `Containerization`: creating a container and running a process inside of it

    Linux kernel provides mechanisms to isolate processes 
    ~
    namespaces isolate processes agains each other, but do not limit access to hardware.

    controlGroup is the one responsible for memory/CPU limitation.

    A container is nothing more than:

    - set of processes
    - each container with a unique namespace
    - processes running inside the container are limited by cgroups

