# Prerequisites

In this lab you will review the machine requirements necessary to follow this tutorial.

## Virtual or Physical Machines

This tutorial requires four (4) virtual or physical x86_64 machines running Debian 12 (bookworm). The following table list the four machines and thier CPU, memory, and storage requirements.

| Name    | Description            | CPU | RAM   | Storage |
|---------|------------------------|-----|-------|---------|
| jumpbox | Administration host    | 1   | 512MB | 10GB    |
| server  | Kubernetes server      | 1   | 2GB   | 20GB    |
| node-0  | Kubernetes worker node | 1   | 2GB   | 20GB    |
| node-1  | Kubernetes worker node | 1   | 2GB   | 20GB    |

How you provision the machines is up to you, the only requirement is that each machine meet the above system requirements including the machine specs and OS version. Once you have all four machine provisioned, verify the system requirements by running the `uname` command on each machine:

```bash 
uname -mov
```

After running the `uname` command you should see the following output:

```text
#1 SMP Debian 6.1.115-1 (2024-11-01) x86_64 GNU/Linux
```

The x86_64 architecture (also known as AMD64) is the 64-bit version of the x86 instruction set. This tutorial will use x86_64 consistently throughout.

Next: [setting-up-the-jumpbox](02-jumpbox.md)
