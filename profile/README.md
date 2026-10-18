<p align="center">
  <img src="https://github.com/moschiten/.github/raw/main/banner.png" alt="Moschito Banner" width="100%">
</p>

# Welcome to Moschiten

Welcome to the official GitHub organization for the Moschito ecosystem. We are building a new standard for containerization that prioritizes universality, portability, and absolute simplicity. 

### What is Moschito

Moschito is a universal, daemonless container ecosystem built entirely from scratch. 

Traditional container engines assume a Linux host, a privileged background daemon, and a shell inside every container. Moschito breaks these assumptions. It is designed to install on any operating system and run containers for any operating system. 

Whether you are on a Linux server, a macOS workstation, a Windows machine, or an Android device, Moschito provides a single, statically compiled Go binary that handles everything. There are no background daemons, no hidden processes, and no bloat.

### Useful Links

Explore the core components of the ecosystem:

**The Core Engine**
- [moschito](https://github.com/moschiten/moschito): The main CLI, builder, and core daemonless engine.
- [midge](https://github.com/moschiten/midge): The universal static PID 1 and execution shim.
- [culicidae](https://github.com/moschiten/culicidae): Custom host backends for Linux, Android, Windows, and macOS.
- [msc](https://github.com/moschiten/msc): The official language specification for Moschito Script.

**Networking and Orchestration**
- [anopheles](https://github.com/moschiten/anopheles): Rootless container networking, virtual Ethernet, and DNS.
- [colony](https://github.com/moschiten/colony): Multi-container deployment and orchestration engine.

**Cloud and Distribution**
- [hive](https://github.com/moschiten/hive): The official OCI registry, image marketplace, and plugin index.
- [get](https://github.com/moschiten/get): Universal installation scripts and package manager manifests.

**Documentation**
- [docs](https://github.com/moschiten/docs): The official documentation website at moschiten.dev.
- [mensch](https://github.com/moschiten/mensch): Source recipes for official trusted base images.

### Feedback

We value the input of the community. If you encounter a bug, have a feature request, or want to discuss the architecture, please use the issue tracker in the relevant repository. For general questions and community discussions, please open a thread in the [moschito discussions](https://github.com/moschiten/moschito/discussions).

### Contributing

Moschito is an open-source project and we welcome contributions of all sizes. Whether you are writing code, improving documentation, or creating new runtime plugins, your help is appreciated. 

To get started, please read our [Contributing Guide](https://github.com/moschiten/moschito/blob/main/CONTRIBUTING.md). All contributors are expected to adhere to our Code of Conduct.

### More

- **Architecture:** Moschito is built on the Moschito Fork-Exec (MFE) model. Every container is a direct child process of the CLI command that started it. 
- **The Language:** We use .msc (Moschito Script), an imperative, 100-command builder language that replaces the Dockerfile, and .colony, a declarative format for orchestration.
- **Security:** By eliminating the root daemon and using direct syscall execution via Midge, we reduce the attack surface of both the host and the container.
- **License:** All projects under the Moschiten organization are licensed under the Apache License 2.0.
