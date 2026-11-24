[![BlackPearl](assets/blackpearl-header.jpg)](https://bpearl.dev/?lang=en)

**🇬🇧 English** · [🇨🇳 简体中文](README.zh-CN.md)

# BlackPearl for Linux

BlackPearl mines Pearl (PRL) on AMD Radeon GPUs. Run it from the command line or use the browser console to configure a multi-GPU rig and monitor each card by its PCIe address.

**143.54 TH/s peak on one Radeon RX 9070 XT** at a 238 W power limit. Four RX 9070 XT cards running together at the same limit delivered **561.82 TH/s combined** in a separate measurement.

**[Download BlackPearl 1.0.10 for Linux x86_64 (75.2 MB)](https://github.com/BlackPearlMiner/bpearl/releases/download/v1.0.10/bpearl-1.0.10-linux-x86_64.tar.gz)** · [SHA-256 checksums](https://github.com/BlackPearlMiner/bpearl/releases/download/v1.0.10/SHA256SUMS) · [Release notes](https://github.com/BlackPearlMiner/bpearl/releases/tag/v1.0.10)

## Performance

| RX 9070 XT configuration | Power limit per GPU | Measured hashrate |
| --- | ---: | ---: |
| One GPU, peak reading | 238 W | 143.54 TH/s |
| One GPU, average over 58.2 seconds | 238 W | 143.44 TH/s |
| Four GPUs, simultaneous readings added together | 238 W | 561.82 TH/s |

These hardware measurements were taken on B85 in November 2026. Combined board power in the four-GPU run was 950 W. The [full benchmarks](https://bpearl.dev/?lang=en#performance) include per-card readings and efficiency across six power limits.

## Install and configure

Version 1.0.10 supports legacy Pearl mining on Ubuntu 24.04 x86_64. The RX 9070 XT requires kernel 6.13 or later, the amdgpu driver and matching firmware. The archive includes the HIP runtime.

Save the archive and checksum file in the same directory, then run:

```sh
sha256sum -c SHA256SUMS &&
  tar xzf bpearl-1.0.10-linux-x86_64.tar.gz &&
  cd bpearl-1.0.10 &&
  sudo ./install.sh
```

Open the address printed by the installer (default `http://127.0.0.1:4088`). Select the GPUs, enter your pool and payout wallet, then check board power, fan speed and temperatures in the console. The developer fee is 0.9% of mining time. The project owner wallet is exempt.

[Installation guide](https://bpearl.dev/en/guide/) · [Download center](https://bpearl.dev/en/downloads/) · [All releases](https://github.com/BlackPearlMiner/bpearl/releases)

## Report an issue

[Open a GitHub issue](https://github.com/BlackPearlMiner/bpearl/issues/new) for installation, GPU detection or mining problems. Include the BlackPearl version, Ubuntu and kernel versions, GPU model and a short log excerpt with credentials removed. [Browse existing issues](https://github.com/BlackPearlMiner/bpearl/issues).
