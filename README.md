<!-- markdownlint-disable MD033 -->
# FranklinNexus

CTO & System Builder. Bridging high-performance infrastructure, hardware-software synergy, and deterministic quant architectures.

[Website](https://www.wisdomechoes.net) · [X/Twitter](https://x.com/FranklinNexus) · [GitHub](https://github.com/FranklinNexus)

<br>

## Core Systems

<table width="100%">
  <tr>
    <td width="72" align="center" valign="top">
      <img src="https://img.icons8.com/ios-filled/50/000000/combo-chart--v1.png" width="36" alt="Quant Terminal">
    </td>
    <td valign="top">
      <b>AlphaHunter (LASZLO)</b><br>
      Omni-asset quant terminal with low-latency research-to-execution routing in Rust and Python.<br><br>
      <a href="https://github.com/FranklinNexus/Omni-Asset-Quant-Terminal">Architecture</a> |
      <a href="https://github.com/FranklinNexus/Omni-Asset-Quant-Terminal">Core Engine</a>
    </td>
    <td width="120" align="right" valign="top">
      <img src="https://img.shields.io/badge/Status-Production-black?style=flat-square" alt="Status">
    </td>
  </tr>
  <tr>
    <td width="72" align="center" valign="top">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/hardware/hardware-original.svg" width="40" alt="Hardware Synergy">
    </td>
    <td valign="top">
      <b>Edge Inference & Hardware Synergy</b><br>
      Profiling LLM inference bottlenecks and quantization paths on FPGA (AX7020) and RISC-V platforms.<br><br>
      Research Notes (WIP)
    </td>
    <td width="120" align="right" valign="top">
      <img src="https://img.shields.io/badge/Stage-Experiment-black?style=flat-square" alt="Stage">
    </td>
  </tr>
  <tr>
    <td width="72" align="center" valign="top">
      <img src="https://img.icons8.com/ios-filled/50/000000/network.png" width="36" alt="Collaborative Network">
    </td>
    <td valign="top">
      <b>SurferGarage 2.0</b><br>
      Permissionless contribution and reputation architecture with transparent routing and anti-fragile design rules.<br><br>
      <a href="https://www.wisdomechoes.net">Ecosystem</a> |
      Protocol Specs (WIP)
    </td>
    <td width="120" align="right" valign="top">
      <img src="https://img.shields.io/badge/Track-Infra-black?style=flat-square" alt="Track">
    </td>
  </tr>
</table>

## Architecture Snapshot

```mermaid
graph TD
    classDef layer fill:none,stroke:#555,stroke-width:1px,stroke-dasharray: 5 5;
    classDef core fill:#111,stroke:#333,stroke-width:1px,color:#fff;
    classDef io fill:#f9f9f9,stroke:#999,stroke-width:1px,color:#000;

    subgraph dp [Data Pipeline]
        A[Market / On-chain Feeds]:::io --> B(Ingestion)
        B --> C(Normalization + Labeling)
    end

    subgraph ae [Alpha Engine]
        C --> D{Signal Engine}:::core
        D -->|Trade Intent| E[Risk Gate]:::core
    end

    subgraph er [Execution Routing]
        E -->|Validation Pass| F[Execution Router]:::core
        F <--> G[(Execution Venue / DEX)]:::io
    end

    F --> H[Telemetry + Post-Trade Analytics]:::io
    H -.->|Model Update / Feedback| D

    class dp,ae,er layer;
```

## Activity

[![GitHub Stats](https://github-readme-stats.vercel.app/api?username=FranklinNexus&show_icons=true&theme=radical&hide_border=true)](https://github.com/FranklinNexus)
[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=FranklinNexus&layout=compact&theme=radical&hide_border=true)](https://github.com/FranklinNexus)
<!-- markdownlint-enable MD033 -->
