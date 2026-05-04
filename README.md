# Green-Box-SpaceRAN


Green Box & SpaceRAN: AvianOS Engineering Suite 🚀
Hard Real-Time Edge AI for Sovereign Urban Infrastructure
This repository contains the technical validation suite for AvianOS, the deterministic kernel powering the Green Box Edge AI gateway. Our architecture bridges the gap between biological reflexes and urban safety through a decentralized "Nervous System" for smart cities.

Project Overview
Green Box & SpaceRAN is an autonomous framework designed to prevent infrastructure failure with zero cloud dependency.

Green Box: An Edge Gateway utilizing AvianOS for sub-millisecond anomaly detection.

SpaceRAN: A sovereign High-Altitude Balloon (HAPS) mesh network for critical "Reflex" communications.

The Technical Suite (Simulation & Testing)
We have provided three distinct C++ implementations to demonstrate the logic, interoperability, and reliability of our system.

1. Basic Reflex Engine (AvianOS_Reflex_Engine.cpp)
Purpose: The Baseline Architecture.

What it proves: Demonstrates the core "Sense-Think-Act" loop. It validates that a local machine can process vibration data and reach a decision without any external server.

Focus: Logic abstraction and basic inference simulation.

2. Integrated Core Demo (AvianOS_Integrated_Core.cpp)
Purpose: The Functional Interoperability Demo.

What it proves: This script demonstrates the full data lifecycle. It detects an anomaly and immediately generates a oneM2M-compliant JSON payload ready for transmission via the SpaceRAN mesh.

Focus: Industry-standard compatibility (oneM2M) and end-to-end data flow.

3. Performance Profiler (AvianOS_Performance_Profiler.cpp)
Purpose: The Engineering Benchmarking Tool.

What it proves: Conducts a statistical stress test over 100 consecutive cycles. It measures Mean, Minimum, and Maximum latency to prove the Determinism of our code.

Focus: Reliability, Jitter analysis, and Hard Real-Time validation (Target: <1ms).

Technical Performance Metrics
Based on our simulation suite, the AvianOS engine has achieved:

Mean Latency: ~21-25 microseconds (Simulation environment).

Determinism: High stability with minimal jitter across multiple trials.

Autonomy: 100% local processing with zero cloud-latency overhead.

How to Build & Run
To ensure industry-grade optimization, we recommend using the O3 flag during compilation:

Bash

# Compile the Integrated Demo
g++ -O3 AvianOS_Integrated_Core.cpp -o Integrated_Demo

# Compile the Performance Profiler
g++ -O3 AvianOS_Performance_Profiler.cpp -o Performance_Profiler


# Run the files
./Integrated_Demo

./Performance_Profiler

System Architecture (AvianOS)

Our software architecture follows the TCA (Think-Connect-Act) Framework:

Sense: Deterministic data acquisition (DMA-ready logic).

Think: Local inference using Quantized AI models (Int8) optimized for NPU acceleration.

Act: Reflex actions triggered via oneM2M standard payloads delivered by SpaceRAN HAPS.

Project Honors
Solo Finalist: 1st Global ESTIMED Hackathon (France).

Award of Excellence: YuKaSong Hackathon 2025.

Scientific Supervision: Under the guidance of Dr. Hatem Zaghloul (Co-inventor of Wi-Fi).
