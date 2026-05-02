# Network Gaming — Performance & Traffic Modelling

> **What real-time multiplayer games actually demand from a network — and what happens when the network can't keep up.**

![Course](https://img.shields.io/badge/SRM%20University-CN%20Project-blue)
![Status](https://img.shields.io/badge/status-research-yellow)
![Year](https://img.shields.io/badge/year-2021-lightgrey)

![SRM](https://user-images.githubusercontent.com/52783096/122576405-499e7200-d06f-11eb-9504-4b372433be3c.png)

---

## About

A 5th-semester Computer Networks project at **SRM University** that surveys and models the traffic real-time multiplayer games push onto packet-switched networks.

- **Who?** A three-person team of CN undergraduates.
- **What?** A literature-driven study + traffic model for real-time multiplayer game flows.
- **Where?** SRM Institute of Science and Technology.
- **When?** Semester 5, 2021 — successor to a prior-semester project ("Distanza").
- **Why?** Voice networks were built for voice. Data networks were built for bulk transfer. Real-time games are neither — and the gap is where lag, jitter, and packet loss live.

## The Story

Multiplayer real-time games are the awkward middle child of network traffic. They demand near-real-time delivery (like voice) but they don't *look* like voice — packets are small, bursty, and bidirectional in unpredictable ways. They also don't look like file transfer: throughput barely matters, latency is everything.

This project digs into three questions:

1. **What do real-time games actually need from a network?** (Latency budgets, packet-loss tolerance, jitter, reordering.)
2. **Can we model the traffic generally?** (One model that survives across genres, parameterized per game.)
3. **What does the market look like?** (Player counts, revenue, gamer classes, willingness to pay — and whether that's enough to drive carriers to upgrade.)

The conclusion line, before the data: cellular networks of the era were *not* tuned for this, and the gap between "minimum playable" and "what the network delivers" is the design space.

## Gallery

> Traffic-trace plots and modelling figures will land here as the analysis is digitized.

---

## Tech Stack

| Layer | Tools |
|------|-------|
| Domain | Computer Networks, traffic modelling, QoS |
| Methods | Literature survey, packet-trace analysis, statistical modelling |
| Output | Research report + (planned) traffic generator |

## Repo Structure

```
Network-Gaming-Performance-and-Traffic-Modelling/
├── LICENSE
└── README.md
```

> Trace data, simulation scripts, and the final paper are kept off-repo for now.

## Getting Started

This is a research/report project, not a runnable codebase. To engage with it:

1. Read the project objectives in this README.
2. Reach out to the authors for the full paper / traces.
3. Use the modelling outline to set up your own ns-3 / iperf experiments.

## Contributing

Open to collaborators interested in:
- Replicating the traffic captures on modern titles (FPS, MOBA, BR).
- Building an open ns-3 module that emits the modelled traffic.
- Updating the QoS thresholds against modern 5G/Wi-Fi 6 measurements.

## License

See `LICENSE`.

## Credits

| Name | GitHub |
|------|--------|
| Gyanesh Samanta | [@GyaneshSamanta](https://github.com/GyaneshSamanta) |
| Ponnu Sharma | [@ponnusharma](https://github.com/ponnusharma) |
| Varsha Narra | [@varsha2612](https://github.com/varsha2612) |

Coursework conducted at **SRM Institute of Science and Technology**.
