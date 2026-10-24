# Mohamed Bekheira

```text
Systems Engineering • Linux Performance • Developer Tools
```

> Exploring Linux internals, performance, and the tools that make systems easier to understand.

I'm a software engineering student at **42 Paris**, with previous experience as a **Systems Engineer Intern at [CodSpeed](https://github.com/CodSpeedHQ)**, where I worked on Linux performance instrumentation, profiling tools, and benchmark runners.

I build tools to **measure Linux behavior**, **diagnose system capabilities**, and **make complex environments easier to understand and reproduce**.

## Working Directory

<p align="center">
  <img src="/assets/working-dir.gif" alt="Working directory animation">
</p>

## Featured Projects

I build these tools under **[DevUtils](https://github.com/devutils-org)** — [explore the projects](https://devutils-org.com/).

### [Omniscient (`omn`)](https://devutils-org.com/tools/omn/) — Linux Profiling & Benchmark Automation

A Rust-based Linux measurement engine for profiling, observability, and **benchmark-as-code** workflows. It collects data directly through **eBPF**, `perf_event_open`, `procfs`, `sysfs`, and netlink—without wrapping external profiling tools.

- **Measurement quality:** provenance, reliability, collection limitations, and cross-subsystem event correlation.
- **Automation:** flexible input and output formats designed to integrate measurements into CI/CD pipelines and reproducible benchmark workflows.

`Rust` · `Linux` · `eBPF` · `perf_event_open` · `Profiling` · `CI/CD` · `Benchmark-as-Code`

**Repository:** Private for now · [Project overview](https://devutils-org.com/tools/omn/)

### [distroproof](https://github.com/devutils-org/distroproof) — Linux Compatibility Diagnostics

A Rust tool for identifying why software behaves differently across Linux environments.

- **Available:** `envprobe`, a static musl-linked CLI that checks kernel capabilities, BPF/perf, security restrictions, libc, and other environment properties; emits diffable JSON reports.
- **VM matrix:** runs a program in QEMU/KVM on 20 distro images, each on its own kernel, and explains failures against passing targets; JSON, JUnit and Markdown reports, and a TUI. Run on Omniscient, it found 27 defects one development machine never showed.

`Rust` · `musl` · `Linux` · `Compatibility` · `JSON`

**Repository:** [devutils-org/distroproof](https://github.com/devutils-org/distroproof) · [Project overview](https://devutils-org.com/tools/distroproof/)

### [atfq](https://github.com/devutils-org/atfq) — Linux Diagnostics & Knowledge

A read-only Linux companion combining **50 live system probes**, an interactive TUI, a built-in knowledge base, JSON output, and a stdio MCP server for AI-agent integration.

- **Focus:** accessible Linux diagnostics without root access, network calls, or system modification.

`Rust` · `CLI` · `TUI` · `procfs` · `sysfs` · `MCP`

**Repository:** [devutils-org/atfq](https://github.com/devutils-org/atfq) · [Project overview](https://devutils-org.com/tools/atfq/)

### [xpac](https://github.com/devutils-org/xpac) — Package Inventory & Reconciliation

A Rust CLI for inspecting installed packages, understanding their provenance and dependencies, and reconciling a machine against declarative TOML profiles.

- **Available:** native package inspection across APT, Pacman, RPM/DNF, Flatpak, Homebrew, apk, and Portage; inventory export, diffs, and reviewable plans.
- **Execution:** experimental, confirmed native execution for all seven; plans can be inspected and dry-run before applying changes.

`Rust` · `CLI` · `TUI` · `Package Management` · `TOML`

**Repository:** [devutils-org/xpac](https://github.com/devutils-org/xpac) · [Project overview](https://devutils-org.com/tools/xpac/)

### [VMAnyware](https://github.com/devutils-org/VMAnyware) — Homelab Infrastructure

An early-stage native application intended to manage reproducible Linux environments on a self-hosted Proxmox homelab.

- **Available:** reusable environment definitions, read-only Proxmox inventory, provisioning previews, and a native SSH terminal prototype with verified host trust.
- **In progress:** confirmed creation, lifecycle, snapshot and deletion workflows pass local fixture checks; real-host validation and a local (QEMU) provider beside Proxmox are next.

`Rust` · `Tauri` · `React` · `Axum` · `Proxmox`

**Repository:** [devutils-org/VMAnyware](https://github.com/devutils-org/VMAnyware) · [Project overview](https://devutils-org.com/tools/vmanyware/)

## Other Engineering Projects

- **[ATFQ Wiki](https://github.com/moha-bekh/atfq-poc)** — Question-driven wiki and learning platform (separate from the Linux diagnostics tool featured above).
- **[WebServ](https://github.com/moha-bekh/WebServ)** — Asynchronous HTTP server in C++: `epoll`, HTTP parsing, CGI, state machines, and memory management.
- **[MiniShell](https://github.com/moha-bekh/minishell)** — Unix shell in C: process management, signals, pipes, expansions, and AST parsing.
- **[libasm](https://github.com/moha-bekh/asm)** — x86-64 Assembly implementations exploring the System V ABI and calling conventions.
- **ft_linux** — Linux From Scratch distribution built from source, including kernel and userspace configuration.
- **[Snow Crash](https://github.com/moha-bekh/snow-crash)** — Linux privilege escalation and security exercises.
- **[Cloud-1](https://github.com/moha-bekh/cloud-1)** — Cloud infrastructure, deployment automation, and Infrastructure as Code.
- **[Inception of Things](https://github.com/moha-bekh/Inception-of-Things)** — Kubernetes fundamentals, container orchestration, and GitOps.
- **[ft_nm](https://github.com/moha-bekh/ft_nm)** — ELF symbol inspection and binary format analysis.
- **[badass](https://github.com/moha-bekh/BADASS)** — Network simulation and configuration with GNS3, Docker, VXLAN, BGP EVPN, and routing protocols.
- **[krpsim](https://github.com/moha-bekh/krpsim)** — Discrete-event simulation, dependency graphs, and scheduling algorithms.
- **[kfs-1](https://github.com/moha-bekh/kernel-from-scratch)** — First steps toward building a small operating system kernel.
- **[miniRT](https://github.com/moha-bekh/miniRT)** — Minimal ray tracer in C exploring ray-object intersections, lighting, and 3D rendering.

## Toolbox

| Area | Technologies |
| --- | --- |
| **Languages** | Rust, C, C++, Go, TypeScript, x86-64 Assembly |
| **Linux & Performance** | POSIX, ELF, `procfs`, `sysfs`, eBPF, `perf_event_open`, profiling |
| **Infrastructure** | Docker, Kubernetes, Terraform, Ansible, AWS, GitHub Actions |
| **Tooling & Interfaces** | CLI, TUI, MCP, Git, JSON output |
| **Environment** | Arch Linux, Neovim, tmux |

<details>
<summary><strong>Interests & reading</strong></summary>

**Engineering interests:** Linux internals, operating systems, performance, kernel development, networking, distributed systems, databases, compilers, and infrastructure.

**On my bookshelf:**
- *Operating Systems: Three Easy Pieces*
- *Computer Systems: A Programmer's Perspective*
- *Low-Level Programming* — Igor Zhirkov
- *The Rust Programming Language*
- *A Philosophy of Software Design* — John Ousterhout
- *Designing Data-Intensive Applications*
- *Code: The Hidden Language of Computer Hardware and Software*

</details>

## Beyond Programming

🏊 Triathlon · 🛹 Action Sports · 🎧 DJing

## Contact

- **Email:** [moha.bekh.pro@gmail.com](mailto:moha.bekh.pro@gmail.com)
- **LinkedIn:** [mohamedbekheira](https://www.linkedin.com/in/mohamedbekheira)
- **GitHub:** [moha-bekh](https://github.com/moha-bekh)
