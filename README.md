# RQMD_RMF_model
The code provides the RQMD.RMF model in Geant4.
The details can be found in https://arxiv.org/html/2503.19395v2.

Usage:<R>
1. unzip RQMDRMF_20250722.zip<R>
```sh
unzip RQMDRMF_20250722.zip
```
2. create the build folder<R>
```sh
mkdir RQMDRMF_20250722-build
cd RQMDRMF_20250722-build
```
3. cmake and make
```sh
cmake -DGeant4_DIR=/Path to Geant4/ ../RQMDRMF_20250722
make 
```
4. run optrun.sh
```sh
chmod u+x optrun.sh
./optrun.sh
```
Then, the cross section data and the corresponding information file (.csv) are created in a new folder (parameter name, i.e. NS2).


