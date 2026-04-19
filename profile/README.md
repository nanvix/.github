# Nanvix: A Microkernel-Based Research Operating System

[![Join us on Slack!](https://img.shields.io/badge/chat-on%20Slack-e01563.svg)](https://join.slack.com/t/nanvix/shared_invite/zt-1yu30bs28-nsNmw8IwCyh6MBBV~B~X7w)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/nanvix/nanvix)
![GitHub last commit](https://img.shields.io/github/last-commit/nanvix/nanvix)
![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/nanvix/nanvix/ci.yml?branch=dev&label=tests)

## Quick Start

### Linux

Requires Ubuntu 24.04 with sudo privileges and
[KVM](doc/setup-linux.md#4-setup-kvm) enabled.

```bash
# Run on Bash.

# Clone main repository.
git clone https://github.com/nanvix/nanvix.git && cd nanvix

# Setup the development environment.
./z setup

# Build Nanvix.
./z build -- all

# Run an example application.
./bin/nanvixd.elf -console-file /dev/stdout -- ./bin/hello-rust-nostd.elf
```

### Windows

Requires Windows 11 with [GNU Make](doc/setup-windows.md#5-run-setup) on PATH, [Windows
Hypervisor Platform](doc/setup-windows.md#4-enable-windows-hypervisor-platform) enabled, [Developer
Mode](doc/setup-windows.md#2-enable-developer-mode) turned on, and a Rust toolchain installed via
[rustup](https://rustup.rs).

```powershell
# Run on PowerShell.

# Clone main repository (symlinks require Developer Mode).
git clone -c core.symlinks=true https://github.com/nanvix/nanvix.git; cd nanvix

# Setup the development environment.
.\z.ps1 setup

# Build Nanvix.
.\z.ps1 build -- all

# Run an example application.
.\bin\uservm.exe -kernel .\bin\kernel.elf -initrd .\bin\hello-rust-nostd.elf -standalone
```

> For more details, see the full [setup](doc/setup.md), [build](doc/build.md), and
> [run](doc/run.md) guides.
  
## How to Join the Community?

Join us on [Slack](https://join.slack.com/t/nanvix/shared_invite/zt-1yu30bs28-nsNmw8IwCyh6MBBV~B~X7w)!
