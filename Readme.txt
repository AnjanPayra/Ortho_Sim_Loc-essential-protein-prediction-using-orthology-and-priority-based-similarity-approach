
1. Sub_cell.py  - Using to calculate subcellular Membership value.
input- Raw file of Sucellular localization (Sub_cellular.txt)
output- Protein wise membership values. Different subcellular files.

2. Get_ess_data.py - Construction of essential dataset.
input- Calculated centrality scores (Centrlity_Ess.csv) and Physicochemical properties score (Physico_chemical_ess.csv). 
output-find protein wise essential dataset (Ess_data.csv)

3. Mem_Cal.py - Membership values of the essential properties.
input- All centrality measures (AllCentrality.xlsx) and All Physicochemical properties ( AllPhysico_chemical.xls)
output-Calculated centrality scores (Centrlity_Ess.csv) and Physicochemical properties score (Physico_chemical_ess.csv).

4. Mem_cen_Sub.py- membership based (alpha, beta, chi, gamma) essential protein prediction based on selected centrality and physico-chemical values.
input- Classifier based calculated centrality properties (Centrlity_Ess.csv) and Physicochemical properties score (Physico_chemical_ess.csv).
output-Essential proteins using membership (alpha, beta, chi, gamma) values.

5.kmeans.py- perform clustering using K-Means clustering.
input- Essential dataset(Ess_data.csv)
output- Clusterwise protein list.

6.Cluster_index.py- Cluster results are validated using validity indices
input-Obtain cluster results from essential dataset.
output- values of the respective validity indices.

7. Sim_loc_score.py- Calculate similarity localized score protein wise.
input-Selected clusters depending on cluster validity indices.
output-protein wise similarity localized score.

8.Thresh_Sim_loc.py- Essential protein prediction using 3-sigma approach
input-protein wise similarity localized score (sim_loc).
output-Three level of threshold(low, mid, high). Essential protein list using thresholds and sim_loc values.

9.level1-2.py,level 1-2_threshold.py , Tot_Socore_levels.py- Find  level-1  proteins of essential proteins using sim_loc values.
input-Protein datasets. sim_loc score of the level-1 proteins of the predicted essential list.
output- predict essential proteins of level-1 of essential list.

10.Ortholog_netComp.py, Fun_subcel_Ortho_list.py- Calculate orthologous value of a protein complex.Listing Ortho_sim_loc properties.
input- Orthologous database, protein database, protein complex.
output- Protein wise orthologous score.

11. Ortho_remove_null.py - Remove proteins without ortholous score.
input- Proteins with orthologous score.
output- Eliminate proteins without orthologous score.

12.Clustering.py- Perform clustering using KMeans, AgglomerativeClustering.
input-Essential dataset(Ess_data.csv).
output-Clusterwise protein list with clustering indices.

13. Physico_chemical.py -Calculate protein wise physico-chemical properties.
input-Protein sequence database.
output-values of different physico-chemical properties values.

14. Diff_Classifier.py -Diff_Classifier to find essential properties of essential dataset
input- All centrality measures and physico-chemical measures.
output-Find selected properties using classifiers.



