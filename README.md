
 ## 🚗 AMMAR (Autonomous Mobility & Multi-Agent Research)


# HPN (Hierarchical Policy Network)
HPN (Hierarchical Policy Network) is a novel hybrid autonomous driving architecture powered by digital twin simulation, designed to overcome the inherent tradeoffs between traditional modular pipelines and monolithic end-to-end driving models. It addresses long-tail rare corner cases in self-driving by splitting driving tasks into tiered expert primitive policies managed by a high-level Arbiter, balancing full safety verifiability, model interpretability, and high driving performance. This framework is validated on CARLA and mainstream autonomous driving digital twin simulators, supporting all common urban, highway, and emergency driving scenarios. details are orividede in :
https://github.com/L221119/HHH123/blob/main/README.md


# LaneGuard (Braking and evasive steering)
a unified end-to-end continuous control framework for autonomous collision avoidance steering that successfully balances aggressive obstacle evasion with mechanical stability, significantly outperforming standard DRL baselines in complex high-speed emergency scenarios.






# LaneAnchor ( Lane Following)
LaneAnchor, an end-to-end imitation learning framework for autonomous lane following that unifies modality-aware cross-modal fusion, navigation-conditioned trajectory decoding, and auxiliary multi-task supervision within a single architecture. Extensive experiments on the \emph{Longest6} benchmark~\cite{chitta2022transfuser} demonstrate its competitive closed-loop performance against representative camera-only and camera-LiDAR fusion methods, while ablation studies further validate the effectiveness of each proposed component. 
source code https://github.com/18haventgirl/LaneAnchor


# CAL-RAPPO ( Intersection Handeling)
CAL-RAPPO is a vision-based deep reinforcement learning project built on the CARLA simulator, designed to enable autonomous driving at unsignalized intersections under adverse weather conditions. The project focuses on end-to-end decision-making in such challenging scenarios. It leverages forward-facing camera images and ego-vehicle states as the primary observation inputs, and trains an agent via a weather-robust perception module coupled with a risk-constrained decision module. This architecture allows the agent to learn adaptive driving strategies that effectively balance safety and efficiency, even in severe weather.

source code: https://github.com/L221119/CAL)


# IST_SACF ( Car Following) 
IST_SACF is a CARLA-based visual reinforcement learning project for safe car-following. The project focuses on single-lane longitudinal car-following. It uses front-view camera images as the main observation input and trains an agent through frame stacking, image augmentation, experience replay, and a contrastive learning auxiliary objective, enabling the agent to learn a stable time-headway control policy while maintaining safety.

 source code https://github.com/howbani/IST-SACF


 # CausalPark (Parking)
  CausalPark: Causal-Aware Dual-Stream End-to-End Autonomous Parking with Multimodal Trajectory Generation
  
  source code https://github.com/howbani/CausalPark




