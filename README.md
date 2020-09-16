# SGX-MR
SGX-MR is a prototype of the paper [SGX-MR: Regulating Dataflows for Protecting Access Patterns of Data-Intensive SGX Applications](https://arxiv.org/abs/2009.03518).

Prototype binaries are provided to test the sample applications described in the paper. 
* KMeans
* WordCount

Binaries are added for both Hardware and Simulation Mode. CPUs without Intel SGX can run binary for simulation mode. 

# Prerequisite
SGX-MR is built on top of intel SGX SDK. To run SGX-MR it is mandetory to install the recent version of SGX SDK. To setup SGX SDK please visit [Linux-SGX](https://github.com/intel/linux-sgx) for detail description.

SGX-MR was built, tested and upload for below configuration:
* 64-bit Ubuntu 18.04.1 LTS (4.15.0 Kernel)
* gcc version 7.5.0
Please ensure the OS and gcc version before testing.


