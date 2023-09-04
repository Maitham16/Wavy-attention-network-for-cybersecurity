# Wavy-attention-network-for-cybersecurity
Wavy-attention network implementation for ICS cybersecurity
# Wavy-Attention Network for Sensor Attack Detection in Nuclear Plants

![Logo or related graphic here](https://github.com/abiodun-ayodeji/Wavy-attention-network-for-cybersecurity/blob/main/Wavenet.png)

Amidst the surge of interest in advanced reactors, especially small modular reactors (SMR) and micro-reactor designs, digitization plays a pivotal role. While digital control systems for these reactors enable optimization, reduced costs, and extended lifetimes, they also introduce potential vulnerabilities to cyberattacks. Our work addresses this risk with the introduction of a **Wavy-Attention Network** designed specifically for sensor attack detection in nuclear plants.

## 🌟 Highlights
- Proposes a **Wavy-Attention Network** for real-time cyber-attack detection in Pressurized Water Reactor (PWR) digital control systems.
- Utilizes the IAEA’s Asherah Nuclear Simulator (ANS) and a false data injection toolbox for model evaluation.
- Achieves **99% accuracy**, outperforming other baseline models like vCNN (90%), LSTM (77%), and Bi-LSTM (91%).


## 🌊 Introducing the Wavy-Attention Network
Traditional deep learning models might fall short when trying to detect subtle cyber threats captured in dynamic sequences of process measurements. Attention mechanisms, especially in transformer architecture, have shown potential in sequence and time-series tasks. However, most of these models cater to large language models and may not be suitable for nuclear plant control signals.

Our **Wavy-Attention Network (WAN)** introduces a sequential self-attention layer in a wavy architecture. This innovative approach captures the dynamic and periodic nature of nuclear control systems, enabling accurate cyber-attack detection.
The model, trained on data simulated from ANS, displays a remarkable **99% accuracy**. For a comprehensive dive into our research, theoretical framework, and results, [refer to the full paper](https://www.ans.org/pubs/proceedings/article-53799/).

## 🛡️ Why Cybersecurity in SMR is Crucial
The advent of digital devices like Programmable Logic Controllers (PLC) and smart sensors brings unprecedented benefits. Yet, the potential cyber vulnerabilities can lead to severe consequences, from plant shutdowns to safety risks. Especially with cyber-physical sensors being susceptible to cyber-attacks targeting specific system frequencies, the need for a robust real-time cyber-attack detection mechanism is more pronounced than ever.


## 🔍 Experiments & Results
Utilizing the Asherah Nuclear Simulator (ANS) in MATLAB/SIMULINK, we simulated conditions for the reactor in its steady state and under attack. Three cyberattacks were simulated on critical sensors, using the [false data injection](https://github.com/sasankapotluri/ICS-Injection_Attack_Toolbox) toolbox developed by Potluri et al. 

Our Wavy-Attention Network classifier was trained, validated, and tested using the data in the repository. The promising results make it evident that WAN holds significant potential for safeguarding future nuclear reactors.

## 🛠️ Getting Started
1. **Installation & Setup**: Please refer to this [notebook](https://github.com/abiodun-ayodeji/Wavy-attention-network-for-cybersecurity/blob/main/WAN_for_ICS_cybersecurity.ipynb) for instructions on dependencies and getting the code running.
2. **Data Preparation**: We have prepared the data for you [here](https://github.com/abiodun-ayodeji/Wavy-attention-network-for-cybersecurity/blob/main/HFA_on_prezz_press.xls), [here](https://github.com/abiodun-ayodeji/Wavy-attention-network-for-cybersecurity/blob/main/HSMI_on_PZ_Level.xls),[here](https://github.com/abiodun-ayodeji/Wavy-attention-network-for-cybersecurity/blob/main/RCA_on_RX_MeanCool.xls) and [here](https://github.com/abiodun-ayodeji/Wavy-attention-network-for-cybersecurity/blob/main/Normal_plant_operation.xls).
3. **Training & evaluation**: Train the Wavy-Attention Network on the provided data using the provided notebook. Or explore better models using the data.

[Detailed Guide & Documentation](https://www.ans.org/pubs/proceedings/article-53799/)


## 📝 Citation
If you find our research useful, please consider citing our paper. Here's a suggested citation format:

Ayodeji A. et al. (2023). Wavy-attention network for real-time cyber-attack detection in a pressurized water reactor digital control system. Proceedings of American Nuclear Society Conference (NPIC&HMIT). Available at: https://www.ans.org/pubs/proceedings/article-53799/

**For direct access to the paper, more insights, deep dives, and discussions, please refer to the [full paper](https://www.ans.org/pubs/proceedings/article-53799/).**
