# Nanvix: A Microkernel-Based Research Operating System

[![Join us on Slack!](https://img.shields.io/badge/chat-on%20Slack-e01563.svg)](https://join.slack.com/t/nanvix/shared_invite/zt-1yu30bs28-nsNmw8IwCyh6MBBV~B~X7w)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/nanvix/nanvix)
![GitHub last commit](https://img.shields.io/github/last-commit/nanvix/nanvix)
![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/nanvix/nanvix/ci.yml?branch=dev&label=tests)

## How to Get Started?

Run these steps on Ubuntu 24.04 with sudo privileges, [Docker](https://github.com/nanvix/nanvix/blob/dev/doc/setup.md#5-setup-docker-optional), and
[KVM](https://github.com/nanvix/nanvix/blob/dev/doc/setup.md#4-setup-kvm) enabled.

```bash
# Clone this source code.
git clone https://github.com/nanvix/nanvix.git && cd nanvix

# Setup a minimal development environment.
./z setup --with-minimal-docker

# Build Nanvix.
./z build --with-minimal-docker -- all

# Run an example application.
./bin/nanvixd.elf -console-file /dev/stdout -- ./bin/hello-rust-nostd.elf
```

> For more details, see the full [setup](https://github.com/nanvix/nanvix/blob/dev/doc/setup.md), [build](https://github.com/nanvix/nanvix/blob/dev/doc/build.md), and
> [run](https://github.com/nanvix/nanvix/blob/dev/doc/run.md) guides.
  
## How to Join the Community?

Join us on [Slack](https://join.slack.com/t/nanvix/shared_invite/zt-1yu30bs28-nsNmw8IwCyh6MBBV~B~X7w)!
