## Neuro-Symbolic approah for the Input and Time Attention Series Prediction

I. Processed JackRabbot dataset (JRDB)
- To download the dataset visit: https://jrdb.erc.monash.edu/
- We trained and tested on scenario: bytes-cafe-2019-02-07_0
- Find processed dataset by navigating to ./scripts/data/JackRabbot/clusters/newest_Nin_1out/ directory, and unzip the "processed_data" folder
- Scripts in qtc_2d and data_processing are used to process the dataset (JRDB) and generate labels. 

II. I/O dataset processing and generation
- Navigate to NeuroSyn-darnn workspace and: catkin_make
- run: rosrun qtc_2d time_series

III. Navigate to the directoty scripts_longterm/ to start the training
To Get started you can run the shell scripts:
- peds_pre_caf_new1.sh for the 48 times steps prediction
- peds_pre_caf_new2.sh for the 80 time steps prediction

IV. To switch between the following models:
- no input attention
- input attention as per the original DA-RNN paper
- input attention with a-priori information on the possible effect of each input time series on the first one (the one we predict), provided by 
the injection of CND-driven attention weights (for human motion prediction application) directly after the series embedding.

please adjust the parameters in the neurosym_train.py:
alpha_update = True/False
inp_att_enabled = True/False
temporal_att_enabled = True/False
run_validation = True/False
run_test = True/False
run_train = True/False

in addition to the hyperparams in the configuraion files in the directory conf/


Note: the generated cnd labels in cnd_labels.txt is a WIP to automatically import them to qtc_indexed_c1.cpp. Currently they are simply copied.
