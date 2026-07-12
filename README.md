# HPN: Hierarchical Policy Network  

🚗 **Part of the AMMAR (Autonomous Mobility & Multi-Agent Research) project**

HPN is a novel hybrid autonomous driving architecture powered by digital-twin simulation.  
It bridges the gap between traditional modular pipelines and monolithic end-to-end models by decomposing driving tasks into **tiered expert primitive policies**, all coordinated by a high-level **Arbiter**.  

This design delivers **full safety verifiability**, **model interpretability**, and **high driving performance** while effectively handling long-tail, rare corner cases.  
The framework is validated on CARLA and other mainstream autonomous driving digital-twin simulators, supporting urban, highway, and emergency scenarios.  

> 📖 **Full architecture details:** [HPN Documentation](https://github.com/L221119/HHH123/blob/main/README.md)

---

## 🔧 Driving Primitives

HPN orchestrates several specialised primitives, each targeting a core driving task:

| Primitive | Task | Description |
|-----------|------|-------------|
| **LaneGuard** | Braking & evasive steering | A unified end-to-end continuous control framework for collision avoidance that balances aggressive obstacle evasion with mechanical stability. Outperforms standard DRL baselines in high‑speed emergency scenarios. |
| **LaneAnchor** | Lane following | An end-to-end imitation learning framework that combines modality‑aware cross‑modal fusion, navigation‑conditioned trajectory decoding, and auxiliary multi‑task supervision. Achieves competitive closed‑loop performance on the *Longest6* benchmark. |
| **CAL‑RAPPO** | Intersection handling | A vision‑based deep reinforcement learning agent for unsignalized intersections in adverse weather. Uses a weather‑robust perception module coupled with a risk‑constrained decision module to balance safety and efficiency. |
| **IST‑SACF** | Car following | Visual RL for safe car‑following. Trained with frame stacking, image augmentation, experience replay, and contrastive learning to learn a stable time‑headway control policy. |
| **CausalPark** | Parking | Causal‑aware dual‑stream end‑to‑end autonomous parking with multimodal trajectory generation. |

### 📂 Source code

- **LaneAnchor** → [github.com/18haventgirl/LaneAnchor](https://github.com/18haventgirl/LaneAnchor)  
- **CAL‑RAPPO** → [github.com/L221119/CAL](https://github.com/L221119/CAL)  
- **IST‑SACF** → [github.com/howbani/IST-SACF](https://github.com/howbani/IST-SACF)  
- **CausalPark** → [github.com/howbani/CausalPark](https://github.com/howbani/CausalPark)  
- *LaneGuard code will be released soon.*

---

## ✨ Key Features

- **Hybrid architecture** – combines modular safety with end‑to‑end flexibility  
- **High‑level Arbiter** – selects the most appropriate expert primitive in real time  
- **Full safety verifiability** – every primitive can be tested and validated independently  
- **Model interpretability** – clear decision boundaries and fallback behaviours  
- **Corner‑case robustness** – specifically designed to master rare, critical scenarios  
- **CARLA & digital‑twin support** – ready to plug into popular simulation environments  

---

## 🚀 Quick Start

### Prerequisites

- [CARLA simulator](https://carla.org/) (0.9.x recommended)  
- Python 3.7+  
- PyTorch, NumPy, OpenCV, etc. (see individual primitive requirements)

### Clone the repository

```bash
git clone https://github.com/L221119/HHH123.git
cd HHH123
