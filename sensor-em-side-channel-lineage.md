# Research Lineage: Sensor Electromagnetic (EM) Side-Channel Leakage

This page maintains a living bibliography of follow-up and closely related work on **sensor electromagnetic (EM) side-channel leakage**. The goal is to give proper credit to all researchers while documenting how the research area has developed.

**EM Eye**, published at NDSS 2024, pioneered the systematic study of content-level electromagnetic side-channel eavesdropping on embedded camera and image-sensor data transmission. By showing that deterministic, unprotected sensor data transmission can induce reconstructable EM leakage, EM Eye laid groundwork for the broader research line on sensor EM side-channel leakage.


## Important Links

- Project website: https://emeyeattack.github.io/Website/
- Official NDSS page: https://www.ndss-symposium.org/ndss-paper/em-eye-characterizing-electromagnetic-side-channel-eavesdropping-on-embedded-cameras/
- Official paper PDF: https://www.ndss-symposium.org/wp-content/uploads/2024-552-paper.pdf
- Code and tutorial: https://github.com/longyan97/EMEye_Tutorial
- HTML lineage page: https://emeyeattack.github.io/Website/sensor-em-side-channel-lineage.html

## Timeline of Follow-up and Closely Related Work

| Year | Work | Sensor modality | Relationship to EM Eye |
| --- | --- | --- | --- |
| 2023 | [FPLogger: Recovering Fingerprints from In-Display Fingerprint Sensors via Electromagnetic Side Channel](https://doi.org/10.1145/3576915.3623153) | In-display fingerprint sensors | Closely related predecessor in biometric EM side-channel leakage. It is listed to give proper credit and to distinguish the broader biometric EM leakage area from the embedded-camera branch pioneered by EM Eye. |
| 2024 | [EM Eye: Characterizing Electromagnetic Side-channel Eavesdropping on Embedded Cameras](https://www.ndss-symposium.org/ndss-paper/em-eye-characterizing-electromagnetic-side-channel-eavesdropping-on-embedded-cameras/) | Embedded RGB cameras and image sensors | Foundational work for content-level EM eavesdropping on embedded camera and image-sensor data transmission. |
| 2025 | [EMIRIS: Eavesdropping on Iris Information via Electromagnetic Side Channel](https://www.ndss-symposium.org/wp-content/uploads/2025-200-paper.pdf) | Near-infrared iris sensors | Follow-up and related work extending EM reconstruction to iris-recognition sensors. |
| 2025/2026 | [EMPalm: Exfiltrating Palm Biometric Data via Electromagnetic Side-Channels](https://arxiv.org/abs/2510.07533) | Palmprint and palmvein sensors | Follow-up and related work extending sensor EM leakage to palm biometric systems. |

## How to Cite EM Eye

Please cite the NDSS 2024 paper when using EM Eye, discussing content-level EM eavesdropping on embedded camera and image-sensor data transmission, or referencing this research lineage.

```bibtex
@inproceedings{long2024emeye,
  title = {EM Eye: Characterizing Electromagnetic Side-channel Eavesdropping on Embedded Cameras},
  author = {Long, Yan and Jiang, Qinhong and Yan, Chen and Alam, Tobias and Ji, Xiaoyu and Xu, Wenyuan and Fu, Kevin},
  booktitle = {Proceedings of the Network and Distributed System Security Symposium (NDSS)},
  year = {2024},
  url = {https://www.ndss-symposium.org/ndss-paper/em-eye-characterizing-electromagnetic-side-channel-eavesdropping-on-embedded-cameras/}
}
```

## BibTeX Entries

A machine-readable bibliography is also available as `followup_works.bib`.

```bibtex
@inproceedings{long2024emeye,
  title = {EM Eye: Characterizing Electromagnetic Side-channel Eavesdropping on Embedded Cameras},
  author = {Long, Yan and Jiang, Qinhong and Yan, Chen and Alam, Tobias and Ji, Xiaoyu and Xu, Wenyuan and Fu, Kevin},
  booktitle = {Proceedings of the Network and Distributed System Security Symposium (NDSS)},
  year = {2024},
  url = {https://www.ndss-symposium.org/ndss-paper/em-eye-characterizing-electromagnetic-side-channel-eavesdropping-on-embedded-cameras/}
}

@inproceedings{ni2023fplogger,
  title = {Recovering Fingerprints from In-Display Fingerprint Sensors via Electromagnetic Side Channel},
  author = {Ni, Tao and Zhang, Xiaokuan and Zhao, Qingchuan},
  booktitle = {Proceedings of the ACM SIGSAC Conference on Computer and Communications Security (CCS)},
  year = {2023},
  doi = {10.1145/3576915.3623153},
  url = {https://doi.org/10.1145/3576915.3623153}
}

@inproceedings{li2025emiris,
  title = {EMIRIS: Eavesdropping on Iris Information via Electromagnetic Side Channel},
  author = {Li, Wenhao and Wang, Jiahao and Zhang, Guoming and Yang, Yanni and Spolaor, Riccardo and Cheng, Xiuzhen and Hu, Pengfei},
  booktitle = {Proceedings of the Network and Distributed System Security Symposium (NDSS)},
  year = {2025},
  url = {https://www.ndss-symposium.org/wp-content/uploads/2025-200-paper.pdf}
}

@misc{xu2025empalm,
  title = {EMPalm: Exfiltrating Palm Biometric Data via Electromagnetic Side-Channels},
  author = {Xu, Haowen and Zhao, Tianya and Wang, Xuyu and Ma, Lei and Dai, Jun and Wyglinski, Alexander and Sun, Xiaoyan},
  year = {2025},
  eprint = {2510.07533},
  archivePrefix = {arXiv},
  primaryClass = {cs.CR},
  url = {https://arxiv.org/abs/2510.07533}
}
```

## FAQ

### Did EM Eye invent all electromagnetic side-channel attacks?

No. Electromagnetic side-channel attacks have a long history, including earlier work on displays, computation, cryptographic devices, and other hardware systems. EM Eye's contribution is more specific: it pioneered the systematic study of content-level EM eavesdropping on embedded camera and image-sensor data transmission.

### Why is EM Eye considered foundational for sensor EM side-channel leakage?

EM Eye showed that deterministic, unprotected sensor data transmission can create image-dependent electromagnetic emissions that allow reconstruction of camera outputs. This root-cause view provided a reusable framework for studying EM leakage from other sensing systems whose data paths may also emit content-dependent signals.

### How is EM Eye related to later iris and palm EM leakage papers?

Later work has extended the broader sensor EM side-channel leakage problem to other sensing modalities, including near-infrared iris sensors, palmprint sensors, and palmvein sensors. These works investigate different sensors and systems, while sharing the broader concern that sensor data transmission can create content-dependent EM emissions.



