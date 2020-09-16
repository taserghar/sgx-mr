# SGX-MR
SGX-MR is a prototype of the paper [SGX-MR: Regulating Dataflows for Protecting Access Patterns of Data-Intensive SGX Applications](https://arxiv.org/abs/2009.03518).

Prototype binaries are provided to test the sample applications described in the paper. 
* KMeans
* WordCount

Binaries are added for both Hardware and Simulation Mode. CPUs without Intel SGX can run binary for simulation mode. 

# Prerequisite
SGX-MR is built on top of intel SGX SDK. To run SGX-MR, it is mandetory to install the recent version of SGX SDK. Please visit [Linux-SGX](https://github.com/intel/linux-sgx) for setup instruction.

SGX-MR was built, tested and upload for below configuration:
* 64-bit Ubuntu 18.04.1 LTS (4.15.0 Kernel)
* gcc version 7.5.0
Please ensure the OS and gcc version before testing.

# Testing
For both Hardware and Simulation mode, a companion shell script (run_sgx-mr.sh) is added to run smaple applications with default parameters. It has four options.
1. kmeans-encoder
2. wc-encoder
3. kmeans-run
4. wc-run
Here, First and second parameters are four generating the block data. For KMeans we generate synthesized data. On the other hand, we used yelp dataset to generate block data for WordCount as we mentioned in the paper. To download yelp data set please visit: https://www.kaggle.com/yelp-dataset/yelp-dataset. In this dataset we set review.json as default input-text. In case of using other text input for wordcount problem, please change the path in the script.
Make sure the data directory along with its sub-directories are also download if using default parameters.

