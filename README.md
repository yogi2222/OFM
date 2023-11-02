Steps to reproduce the results:

Step 1.  ofm-Mn-git1.csv and ofm-Mn-git2.csv contain the input data for training the model to predict the formation energy per atom and magnetic moment per atom(Mperatom). Due to upload file size restrictions, data is divided into two parts. The combined data of both files is used for model training. This data can also be generated using the code make-ofm.ipynb.

Step 2.  predict-new-materials.ipynb code is used to predict new materials. It needs two input files (1) ofm-mn-all.csv; This can be made by combining ofm-Mn-git1.csv and ofm-Mn-git2.csv files (2) EuMnIn.vasp (given here); this is a structure file used in vasp. It can also be downloaded from the materials project. We can replace this file with the desired one to get the formation energy per atom and magnetic moment per atom of that type of materials. In this file, we have substituted all available atoms in the place of In atom and predicted the formation energy per atom and magnetic moment per atom of all combinations using the code "predict-new-materials.ipynb". 

Step 3. All predicted data will be saved in the "data1.csv" file. Select the desired materials with a high magnetic moment and negative formation energy.

Step 4. Replace the "EuMnIn.vasp" file with the desired file and get the properties of the materials.

Using "predict-new-materials.ipynb" code, one can substitute any atom in any material at any position and then predict the formation energy per atom and magnetic moment per atom of the substituted material.

