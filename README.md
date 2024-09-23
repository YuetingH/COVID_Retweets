# COVID_Retweets

## Repo Structure
```bash
COVID_Retweets
¦   README.md   
¦   requirements.txt
¦   1_Graph_Filter_vs_Unfiltered.ipynb              # Fig 1 in paper
¦   2_Retweets_vs_Followers.ipynb                   # Fig 2 & 3
¦   3_Temporal_Bowtie.ipynb                         # Fig 4 & 5
¦   Graph_Demo.ipynb                                # instructions: import & extract temporal (sub)graphs
¦   SM_Data_Import+Cleaning+SummaryStats.ipynb      # SM: original retweet data preprocessing
¦
+--- Data (not public available)
¦   ¦   original_data.dat
¦   ¦   dataCleaning_indexRetain.pickle
¦
+--- Graphs (not public available)
¦   ¦   G_original.gpickle                          # the original network aggregating the entire data timeframe - a directed weighted network with attributes
¦   ¦   G_original_unattributed                     # an unattributed version for faster loading
¦   ¦   G_filtered.gpickle                          # filtering the original network by retaining statistically significant edges only
¦   ¦   G_filtered_sub1.gpickle                     # filtered subgraph (6 months: 2020-09-17 to 2021-03-17)
¦   ¦   G_filtered_sub2.gpickle                     # filtered subgraph (6 months: 2021-11-17 to 2022-05-17)
¦   ¦   newsCateogry_dict_decode.pickle             # for retrieving retweets' cateogories (converted into integers when constructing graphs to save storage)
¦   ¦   newsCateogry_dict_generalised_code.pickle   # for generalising cateogories into 'scientific', 'fake', 'uncertain' 
¦   ¦   user_dict_decode.pickle                     # for retrieving users' IDs (converted into integers when constructing graphs to save storage)
¦
+--- Results (not public available)                 # store some time-consuming results
¦   ¦   ... 
¦
+--- Figures
¦   ¦   ...                                         
             
```




