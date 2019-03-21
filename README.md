# Linux Container Fundamentals

This repo contains an outline and (eventually) a script for a series of videos,
likely 15 minutes in length each, explaining the fundamental components of Linux
containers at a high level. Each component will be demonstrated in isolation.

I hope to create the video series in the style of Khan academy; a voice over of
drawing with interludes into a terminal.

## Topics

- Introduction
  - What is a container?
  - Why use containers?
  - Open Containers Initiative and runc
- Control Groups
  - Control over physical resources
  - `cpu`/`cpuset`/`cpuacct`, `memory`, `net`/`net_cls`, `blkio`
  - Control over virtual resources
  - `devices`, `freezer`, `pids`, `hugetlb`
- Namespaces (2 parts?)
  - Isolation of virtual resources
  - `unshare`, `clone` and `setns`
  - `mnt`, `pid`, `net`, `ipc`, `uts`
  - `user` and `uid_map`
- Container Filesystems (2 parts?)
  - `pivot_root`
  - Mounts
  - Layered filesystems
  - Filesystem quotas
  - Masked paths
- Capabilities
  - What is root really?
  - Inspecting capabilities
  - `capset` and restricting capabilities
  - `setcap` and file capabilities
  - Dropping capabilities
- AppArmor
- Seccomp
