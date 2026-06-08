# IOT-security-thesis
# Internet of Things Security

**Author:** Katta Sathvik Reddy  
**Institution:** Birla Institute of Technology and Science (BITS), Pilani — Hyderabad Campus  
**Supervisor:** Dr. Jay Kamlesh Dave  
**Date:** December 2024

---

## Overview

This thesis presents a comprehensive study of Internet of Things (IoT) security — analyzing the threat landscape, existing defense mechanisms, real-world attack case studies, and ML/DL-based Intrusion Detection Systems. It also proposes LAKE-ECC, a lightweight cryptographic protocol designed to address a key gap identified through the survey.

---

## Contents

- IoT architecture overview and layer-wise security analysis across the perception, network, and application layers
- Classification of 20+ attack types including DDoS, MITM, Sinkhole, Wormhole, Sybil, Node Capture, Replay, Side-Channel, and RFID-based attacks
- Real-world IoT breach case studies: Mirai Botnet, Stuxnet, Verkada camera hack, St. Jude Medical cardiac implant vulnerability, VPNFilter malware, Tesla Model X hack, and the Jeep Cherokee remote hijack
- Comparison of cloud vs. edge vs. hybrid computing architectures for IoT data processing
- Review of existing IoT security solutions: Blockchain, Fog Computing, SDN, Lightweight Cryptography, Zero Trust Architecture, and Digital Twins
- Survey of 15+ ML/DL-based Intrusion Detection System (IDS) models including Naive Bayes, KNN, SVM, Decision Trees, Random Forest, CNN, RNN, LSTM, GAN, Deep Autoencoders, DBN, and Ensemble methods
- Critical evaluation of 11 public IoT security datasets: NSL-KDD, BoT-IoT, UNSW-NB15, N-BaIoT, CICIDS2017, KDD99, and others
- Analysis of open research challenges: dataset quality, real-time detection complexity, model bias, device heterogeneity, privacy concerns, and scalability
- Discussion of future prospects: federated learning, post-quantum encryption, zero-touch onboarding, embedded security-by-design, and AI-driven threat detection
- Proposed Protocol: LAKE-ECC — a lightweight authenticated key exchange protocol for resource-constrained IoT devices using ECC, Schnorr signatures, and Mahalanobis distance anomaly detection
---

## Research and proposed solutions
Designed LAKE-ECC, a novel lightweight authenticated key exchange protocol for resource-constrained IoT devices using ECDH over NIST P-256, Schnorr signatures, and BLAKE2s key derivation, achieving mutual authentication and Perfect Forward Secrecy within a 242-byte message footprint — comparable to a single ZigBee frame
Proposed a Mahalanobis distance-based behavioral anomaly detection layer at the gateway level to identify relay and wormhole attacks using chi-squared statistical thresholding on per-device handshake fingerprints
Formally analyzed LAKE-ECC security under the Canetti-Krawczyk (CK) threat model, proving resistance to replay, man-in-the-middle, and session linkage attacks grounded in the Elliptic Curve Discrete Logarithm Problem (ECDLP)

Benchmarked LAKE-ECC computational feasibility across ARM Cortex-M0, Cortex-M4, and ATECC608 hardware co-processor targets, estimating full handshake times of ~12s (Cortex-M0 SW), ~1.2s (Cortex-M4 SW), and ~560ms (hardware accelerated)
Compared LAKE-ECC against TLS 1.3, DTLS 1.3 with PSK, and IETF EDHOC (RFC 9528) across forward secrecy, PKI requirements, message size, and authentication mechanism, demonstrating superior resource efficiency with equivalent security guarantees
Evaluated trade-offs between cloud and edge computing for IoT data processing across latency, scalability, privacy, and bandwidth dimensions, contributing to architectural recommendations for hybrid IoT deployments


## Technologies & Concepts

`IoT Security` `IDS/IPS` `Machine Learning` `Deep Learning` `CNN` `RNN` `LSTM` `GAN` `Random Forest` `SVM` `Blockchain` `Edge Computing` `Fog Computing` `Federated Learning` `SDN` `Zero Trust` `ECC` `AES` `TLS` `DTLS` `MQTT` `CoAP` `ZigBee` `6LoWPAN` `LoRaWAN`
ECC (NIST P-256) · ECDH · Schnorr Signatures · BLAKE2s · AES-128-CCM · Mahalanobis Distance · Chi-Squared Testing · TLS/DTLS · SVM · IDS/IPS

---

## File

| File | Description |
|---|---|
| `IoT_Security_Thesis.pdf` | Full thesis report |

---

*Submitted in partial fulfillment of the requirements of BITS F423T/424T Thesis, BITS Pilani Hyderabad Campus, December 2024.*
