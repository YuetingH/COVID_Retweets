# COVID_Retweets

## Repo Structure
```bash
COVID_Retweets
¦   README.md   
¦   requirements.txt
¦   1_Graph_Filter_vs_Unfiltered.ipynb              # Fig 1 in paper
¦   2_Retweets_vs_Followers.ipynb                   # Fig 2
¦   3_Temporal_Bowtie.ipynb                         # Fig 3 & 4
¦   Graph_Demo.ipynb                                # instructions: import & extract temporal (sub)graphs
¦   SM_Data_Import+Cleaning+SummaryStats.ipynb      # SM: original retweet data preprocessing
¦
+--- Data (not public available)
¦   ¦   original_data.dat
¦   ¦   dataCleaning_indexRetain.pickle
¦
+--- Graphs (not public available)
¦   ¦   G_original.gpickle                          # retweet network aggregating the entire data timeframe - a directed weighted network with attributes
¦   ¦   G_original_unattributed                     # an unattributed version for faster loading
¦   ¦   G_filtered.gpickle                          # filtered retweet network by retaining statistically significant edges only
¦   ¦   G_filtered_sub1.gpickle                     # filtered retweet netowork (5 months: 2020-11-17 to 2021-04-17)
¦   ¦   G_filtered_sub2.gpickle                     # filtered retweet netowork (5 cmonths: 2021-11-17 to 2022-04-17)
¦   ¦   newsCateogry_dict_decode.pickle             # for retrieving retweets' cateogories 'CLICKBAIT', etc.(converted into integers when constructing graphs to save storage)
¦   ¦   newsCateogry_dict_generalised_code.pickle   # code of generalised cateogories 'scientific', 'fake', 'uncertain'
¦   ¦   user_dict_decode.pickle                     # for retrieving users' ID 
¦
+--- Results (not public available)                 # store some time-consuming results
¦   ¦   ... 
¦
+--- Figures
¦   ¦   ...                                         
             
```




