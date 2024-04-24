# OSSL
[IJCAI2024] Dynamic Against Dynamic: An Open-set Self-learning Framework

*********************************************************************
Code of Dynamic Against Dynamic: An Open-set Self-learning Framework.
This foler contains an example the training and testing code for the open-set recognition experiment conducted on TinyImageNet.
Enjoy the code.

**************************** Requirement ****************************

#requirement Python3.8.16, PyTorch1.12.1

******************************* USAGE *******************************

data ----- This folder is used to store specific datasets, including text files containing dataset paths.

log  ----- By default, the saved model parameters exist in this folder and are then used for various operations such as testing phase. Of course, the file path for saving model parameters can also be customized in the code.

models ----- Under this folder, some of the neural networks used are stored. The neural networks in this folder, along with the net.py file, constitute the network architecture of the OSSL framework.

main.py ---- The main file used for operation during the training and testing phase.

tinyimagenet-train-config.yaml and tinyimagenet-test-config.yaml ----

For the training and testing configuration file of the TinyImageNet dataset, it is necessary to specify the experimental dataset and its path. At the same time, specific values such as batch size and file paths such as the starting classifier need to be specified in this file.

--A. Training and test script
download datasets;
write your config file and run the code as:
python main.py --config /path/to/your/config/yaml/file
train :
python main.py --config tinyimagenet-train-config.yaml
test:
python main.py --config tinyimagenet-test-config.yaml


--B. Data organization
All the experimental datasets are widely used datasets for open access, which can be easily obtained.
The datasets' spils of known and unknown are shown in osr_split.py


***************************** REFERENCE *****************************

If you use this code in scientific work, please cite: 

Haifeng Yang*, Chuanxing Geng*, Pong C. Yuen and Songcan Chen. Dynamic Against Dynamic: An Open-set Self-learning Framework.
In: Proceedings of the 33th International Joint Conference on Artificial Intelligence (IJCAI'24).
*********************************************************************
