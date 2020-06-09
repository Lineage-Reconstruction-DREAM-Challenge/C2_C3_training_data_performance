### Comparing the performance on the training data for Challenge 2.
For the performance on the Challenge 2 training data,  please upload a tab-delimited file with three columns: 
1. sample ID (from 1 to 100)
2. normalized RF distance
3. normalized triplet distance between the ground truth tree and predicted tree 

* K-mer replacement distance (Kwak_Gong): [challenge=C2_group=Kwak_Gong.v2.tsv](challenge=C2_group=Kwak_Gong.v2.tsv)
* GuanLab: [challenge=C2_group=GuanLab.tsv](challenge=C2_group=GuanLab.tsv)
* Jingyuan: [challenge=C2_group=Jingyuan_Hu.tsv](challenge=C2_group=Jingyuan_Hu.tsv)
* Weighted hamming (Kwak_Gong): [challenge=C2_group=Kwak_gong_weighted_hamming_TreeCmp.tsv](challenge=C2_group=Kwak_gong_weighted_hamming_TreeCmp.tsv)
* Yosef Lab: [challenge=C2_group=MJ.tsv](challenge=C2_group=MJ.tsv)
* Renata's method: [challenge=C2_group=AMbeRland.tsv](challenge=C2_group=AMbeRland.tsv)

Script for computing the RF distance and triplet distance between groud truth tree and predicted tree: 
https://github.com/Sage-Bionetworks/Allen-DREAM-Challenge/blob/master/Docker/score.py

Example notebook for computing RF distance and triplet distance using TreeCmp: https://github.com/ofirr/dream_examples/blob/master/treecmp_comparison_example.ipynb

### Benchmarking running time 
Each method will be tested on one randomly generated dataset of [1,000 cells with 200 targets](https://s3.msi.umn.edu/gongx030/rlib/C2_C3_training_data_performance/C2_test.tsv), and one dataset of [2,500 cells with 1,000 targets](https://s3.msi.umn.edu/gongx030/rlib/C2_C3_training_data_performance/C3_test.tsv). 

Here are a list of jupyter notebooks for the benchmark:
* Cassiopeia-Greedy: [Cassiopeia_C2.ipynb](Cassiopeia_C2.ipynb), [Cassiopeia_C3.ipynb](Cassiopeia_C3.ipynb)
* DCLEAR(WHD): [DCLEAR_WHD_C2.ipynb](DCLEAR_WHD_C2.ipynb), [DCLEAR_KRD_C3.ipynb](DCLEAR_WHD_C3.ipynb)
* DCLEAR(KRD): [DCLEAR_KRD_C2.ipynb](DCLEAR_KRD_C2.ipynb), [DCLEAR_KRD_C3.ipynb](DCLEAR_WHD_C3.ipynb)
* Liu's method: [Liu_C2.ipynb](Liu_C2.ipynb), [Liu_C3.ipynb](Liu_C3.ipynb)
* Guan's method: [Guan_C2.ipynb](Guan_C2.ipynb), [Guan_C3.ipynb](Guan_C3.ipynb)
* FastTree2: [FT2_C2.ipynb](FT2_C2.ipynb), [FT2_C3.ipynb](FT2_C3.ipynb)

Each notebook was run on a standard Google Colab node with two 2.2G Hz Xeon CPUs. 
