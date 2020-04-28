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

Script for computing the RF distance and triplet distance between groud truth tree and predicted tree: 
https://github.com/Sage-Bionetworks/Allen-DREAM-Challenge/blob/master/Docker/score.py

Example notebook for computing RF distance and triplet distance using TreeCmp: https://github.com/ofirr/dream_examples/blob/master/treecmp_comparison_example.ipynb

