# Renaming 
Notebooks in this folder are the final step in renaming features with the new updated gene lists to ensure synchronised features prior to integration. 

Using Seurat's **UpdateSymbolList()** function, I retrieved an updated gene list according to the HGNC database. The main challenge here was the duplicates. Duplicates were either false duplicates; in this case the original names were kept, or, duplicates were true; in this case the rows were collapsed and their signal count was summed. 

In these notebooks, Seurat objects were created with the new gene names, duplicated were found, and aggregated into single rows. The object was then saved as final object, ready for integration. 
