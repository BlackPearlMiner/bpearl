# BlackPearl 1.0.10 安装说明

适用系统为 Ubuntu 24.04 x86_64。RX 9070 XT 需要 Linux 6.13 或更新内核、amdgpu 驱动和配套固件。安装包随附 HIP 用户态运行库。

1. 从[正式版下载页](https://github.com/BlackPearlMiner/bpearl/releases/tag/v1.0.10)下载 `bpearl-1.0.10-linux-x86_64.tar.gz` 与 `SHA256SUMS`，放到同一个目录。
2. 在该目录校验文件。确认显示 `OK` 后解压并安装。

   ```sh
   sha256sum -c SHA256SUMS &&
     tar xzf bpearl-1.0.10-linux-x86_64.tar.gz &&
     cd bpearl-1.0.10 &&
     sudo ./install.sh
   ```

3. 打开安装器打印的控制台地址，默认是 `http://127.0.0.1:4088`。在配置向导核对显卡、矿池和自己的收款钱包。

[完整安装手册与故障排查](https://bpearl.dev/guide/) · [English installation guide](https://bpearl.dev/en/guide/)
