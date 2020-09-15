# Continuous Conditional GAN (CcGAN)

If you use this code, please cite
```text
placeholder...
```


# 1. Datasets
## RC-49 Dataset (h5 file)
https://1drv.ms/u/s!Arj2pETbYnWQr7MY2Pr5qipSUpZKEQ?e=k8HfB6

Download 'RC-49_64x64.h5' and put it in './CcGAN/dataset/RC-49'

## modified UTKFace Dataset (h5 file)
https://1drv.ms/u/s!Arj2pETbYnWQr7MW_sGY9tJC4G3eMw?e=gmTA0w

Download 'UTKFace_64x64.h5' and put it in './CcGAN/dataset/UTKFace'


# 2. Sample Usage
## 2.1 Simulation ('./CcGAN/Simulation')
First, set the ROOT_PATH in the 'run_train.sh' to yours. 

Then, run 'run_train.sh'.


## 2.2 RC-49 ('./CcGAN/RC-49')
First, set the ROOT_PATH and DATA_PATH in the 'run_train.sh' to yours. 

Then, run 'run_train.sh'.


## 2.3 UTKFace ('./CcGAN/UTKFace')
First, set the ROOT_PATH and DATA_PATH in 'run_train.sh' to yours. 

Then, run 'run_train.sh'.


# 3. Some results

## 3.1 Simulation: Circular 2-D Gaussians
### Training data
<img src="./images/Simulation/samples_train_with_means_nSim_0.png" alt="Trainin data" height="400" width="400"/> 

### cGAN
<img src="./images/Simulation/cGAN_real_fake_samples_nSim_0.png" alt="cGAN" height="400" width="400"/>

### HVDL
<img src="./images/Simulation/CcGAN_real_fake_samples_hard_nSim_0.png" alt="HVDL" height="400" width="400"/>

### SVDL
<img src="./images/Simulation/CcGAN_real_fake_samples_soft_nSim_0.png" alt="HVDL" height="400" width="400"/>


## 3.2 RC-49
### Visual Comparison
<img src="./images/RC-49/RC49_comparison.png" alt="Visual Comparison" height="500" width="600"/> 

### FID vs Angle
<img src="./images/RC-49/RC49_comparison_fid_versus_center_vanilla.png" height="400" width="600"/> 

### NIQE vs Angle
<img src="./images/RC-49/RC49_comparison_NIQE_versus_center_vanilla.png" height="400" width="600"/> 

### Diversity vs Angle
<img src="./images/RC-49/RC49_comparison_diversity_versus_center_vanilla.png" height="400" width="600"/> 



## 3.3 UTKFace
### Visual Comparison
<img src="./images/UTKFace/UTKFace_comparison.png" alt="Visual Comparison" height="500" width="600"/> 

### FID vs Angle
<img src="./images/UTKFace/UTKFace_comparison_fid_versus_center_vanilla.png" height="400" width="600"/> 

### NIQE vs Angle
<img src="./images/UTKFace/UTKFace_comparison_NIQE_versus_center_vanilla.png" height="400" width="600"/> 

### Diversity vs Angle
<img src="./images/UTKFace/UTKFace_comparison_diversity_versus_center_vanilla.png" height="400" width="600"/> 
