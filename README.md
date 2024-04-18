# Progressive Contextual Trajectory Prediction with Adaptive Gating and Fuzzy Logic Integration
Despite the rapid advancement of highly automated vehicles poised to mitigate accidents caused by human errors, understanding the behaviors of road users, especially vulnerable pedestrians, remains a significant challenge. The evolution of pedestrian trajectory prediction, transitioning from early motion models to recent deep learning approaches, has highlighted persistent challenges in accurately predicting future trajectories, particularly in complex scenarios. To address this, this paper presents a Progressive Contextual Trajectory Prediction with Adaptive Gating and Fuzzy Logic Integration (PCTP-AGFL). The proposed method incorporates a dynamic progressive generator (DPG) comprising multiple LSTM layers that adapt progressively to pedestrian motion pattern complexities. The DPG is trained using a learned scheduled sampling strategy implemented through an Adaptive Gating Mechanism (AGM), allowing dynamic switching between teacher forcing and normal mode. This is augmented with an Encoder-Decoder Contextual Attention (EDCA) module to enhance contextual awareness. Additionally, a novel Adaptive Fuzzified Discriminator (AFD) is introduced to enhance the model's capability to handle ambiguous trajectories. Experimental results on JAAD/PIE and ETH/UCY datasets demonstrate the method's superiority over baselines and state-of-the-art approaches. Furthermore, a comprehensive ablation study is carried out to tune the progression parameters, training strategy, and the type of classifier logic in the discriminator.
![image](https://github.com/neha013/PCTP-AGFL/assets/41139808/34aef85b-8449-4467-b42b-e79bb6788beb)
Proposed trajectory prediction architecture. P_n denotes the observed trajectory of a pedestrian at time step 'n,' based on the previous 'k' timesteps, P_n={p_(n-k+1),p_(n-k+2),…,p_n}, where 'p_n' encompasses top-left (x_tl,y_tl) and bottom-right (x_br,y_br) bounding box coordinates. The goal is to predict 'ν' future coordinates Q_n={y_(n+1),y_(n+2),…,y_(n+ν)}. It employs a Dynamic Progressive generator (DPG) framework that allows dynamic switching between training strategies yielding different decoder inputs Q_n^NMand Q_n^TF for normal mode and teacher forcing modes respectively. The context vector C_m for the m^th decoder timestep is enhanced by integrating the Encoder-Decoder Contextual Attention (EDCA) module output, pedestrian ROIs R_n={r_(n-k+1),r_(n-k+2),…,r_n}, and segmentation maps  S_n={s_(n-k+1),s_(n-k+2),…,s_n}. An Adaptive Fuzzified Discriminator (AFD) further enhances classification accuracy for ambiguous trajectories
