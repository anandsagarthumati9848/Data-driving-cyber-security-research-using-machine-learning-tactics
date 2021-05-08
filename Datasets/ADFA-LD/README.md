# ADFA-LD Data Description:

In 2013, the University of New South Wales at the Australian Defense Force Academy developed 2 new datasets that are ADFA-LD and ADFA-WD. The first one includes host-based and network-based intrusion datafrom a Linux operating system version 11.04, whereas the second one includes data from a Window operating system.The host-based dataset contains 3 files: training, validating and testing set. Since it is designed for an anomaly-based intrusion detection, the training and validating sets were collected during normal activities, where there were only normal sequences. On the other hand, testing set contains only intrusion sequences from various attacks including password brute force, web-based attacks and remote exploits. These attacks are conducted by penetration testers and hackers, and it representscurrent cyberattack strategies. There are 6 types of simulated attacks, and the testing set contains 10 attacks per type.
The main difference between datasets from ADFA versus from UNM is the data format. The ADFA dataset contains only traces of system call number different programs. Additionally, there is no PID nor time stamp for each system call in ADFA data. 

# Data Usage:

Since there are more than enough normal data from the training dataset, we only Training_Data_Master.zip and Attack_Data_Master.zip files. We randomly choose 7000 normal sequences and 7000 intrusion sequences to create a sample pool and split them into a training and testing sets with a 70-30 ratio.

To run the candidate algorithms with ADFA-LD dataset, open HIDS-ADFA.ipynb in Google Colab and load Training_Data_Master.zip and Attack_Data_Master.zip files. Select Runtime and then Run All to run all blocks of codes. You should see results from each code block as the python notebook is running. 
