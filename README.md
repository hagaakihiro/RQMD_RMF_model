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
Then, the cross section data and the corresponding information file (.csv) are created in a new folder (parameter name, e.g. NS2).

optrun.sh runs all projectile-target combonatinos listed in projectile.txt;
```txt
50.13,0.05,6,12,1,1,LIQMD
```
means incident energy, and its standard deviation (MeV/nucleon), projectile Z, projectile A, target Z, target A, and text (not used).
The number of incidnet particles is set as 100,000 (line 256 in pencil_ion.cc), and its simulation is repeated by N defined in optrun.sh.



