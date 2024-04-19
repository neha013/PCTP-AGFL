# Progressive Contextual Trajectory Prediction with Adaptive Gating and Fuzzy Logic Integration
This is the official python implementation for paper, *[Progressive Contextual Trajectory Prediction with Adaptive Gating and Fuzzy Logic Integration](https://www.google.com "Google's Homepage")*. authored by ***Neha Sharma, Chhavi Dhiman, S. Indu***
![image](https://github.com/neha013/PCTP-AGFL/assets/41139808/34aef85b-8449-4467-b42b-e79bb6788beb)
Despite the rapid advancement of highly automated vehicles poised to mitigate accidents caused by human errors, understanding the behaviors of road users, especially vulnerable pedestrians, remains a significant challenge. The evolution of pedestrian trajectory prediction, transitioning from early motion models to recent deep learning approaches, has highlighted persistent challenges in accurately predicting future trajectories, particularly in complex scenarios. To address this, this paper presents a Progressive Contextual Trajectory Prediction with Adaptive Gating and Fuzzy Logic Integration (PCTP-AGFL). The proposed method incorporates a dynamic progressive generator (DPG) comprising multiple LSTM layers that adapt progressively to pedestrian motion pattern complexities. The DPG is trained using a learned scheduled sampling strategy implemented through an Adaptive Gating Mechanism (AGM), allowing dynamic switching between teacher forcing and normal mode. This is augmented with an Encoder-Decoder Contextual Attention (EDCA) module to enhance contextual awareness. Additionally, a novel Adaptive Fuzzified Discriminator (AFD) is introduced to enhance the model's capability to handle ambiguous trajectories. Experimental results on [JAAD](http://data.nvision2.eecs.yorku.ca/JAAD_dataset/)/[PIE](http://data.nvision2.eecs.yorku.ca/PIE_dataset/) and [ETH](https://icu.ee.ethz.ch/research/datsets.html)/[UCY](https://graphics.cs.ucy.ac.cy/portfolio) demonstrate the method's superiority over baselines and state-of-the-art approaches. Furthermore, a comprehensive ablation study is carried out to tune the progression parameters, training strategy, and the type of classifier logic in the discriminator. 
