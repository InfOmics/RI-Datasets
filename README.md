# RI-Datasets

Available datasets are distributed under the RI project license and can be requested by email.

<hr />

### AIDS
>small molecules

AIDS dataset contains the topological structures of 40000 chemical compounds that have been tested for evidence of anti-HIV activity (available from NCBI). Compounds are undirected graphs where the number of vertices varies from 4 to 245. They are small sparse graphs. 
Since the AIDS dataset contains relatively small graphs, the patterns are graphs of the dataset. Patterns were divided into four groups, each group has 100 graphs, and each graph may have 4, 8, 16 or 32 vertices. The topology of patterns was chosen in order to respect the average degree and label distribution of the target graphs. This implies that patterns were often quite complex. 
[National Cancer Institute]( http://www.nci.nih.gov/)

### PDBSv1 
>proteins,large sparse graphs

This dataset contains 30 graphs with data from DNA, RNA, and proteins having up to 33067 vertices. Original structures can be downloaded from the JenaLib and RCSB. Downloaded molecules in PDB format were converted in graphs using BALL. The dataset mostly contains large sparse graphs. 
Pattern graphs were extracted from the corresponding target graphs fixing the number of wanted edges. Patterns are subgraphs (monomorphisms) of their corresponding target graphs. We create six groups of 10 random patterns having a number of edges equals to 4, 8, 16, 32, 64, and 128. 

[Huehne R, Suehnel J: The Jena Library of Biological Macromolecules. Nature-precedings 2009.] <br>
[Protein Data Bank]( http://www.rcsb.org/pdb/.) <br>
[Boghossian N, Kohlbacher O, Lenhof H: BALL: Biochemical Algorithms Library. In Proceeding of the 3rd workshop on algorithms engineering WAE 99 Lecture Notes in Computer Science, 1668, Springer, Berlin, London, UK, pp. 330-344, 1999.]

### PDBSv2
>protein backbones,medium sparse graphs

This dataset contains 40 proteins represented by the backbones of the proteins coming from the crystallography downloaded from JenaLib and RCSB. converted to graphs by BALL library . They are medium sparse graphs. They may have from 1683 to 7979 vertices per graph. 
Pattern graphs were extracted from the corresponding target graphs as we have done for dataset PDBSv1. We create seven groups of 10 random patterns, re ecting the typology of the target graphs, having a number of edges equals to 4, 8, 16, 32, 64, 128 and 256. 

[Huehne R, Suehnel J: The Jena Library of Biological Macromolecules. Nature-precedings 2009.] <br>
[Protein Data Bank]( http://www.rcsb.org/pdb/.) <br>
[Boghossian N, Kohlbacher O, Lenhof H: BALL: Biochemical Algorithms Library. In Proceeding of the 3rd workshop on algorithms engineering WAE 99 Lecture Notes in Computer Science, 1668, Springer, Berlin, London, UK, pp. 330-344, 1999.]

### PDBSv3
>protein contacts maps,small dense graph

This dataset contains 50 contact maps of the amino acids of the domains of the proteins, retrieved by CMView. They represent relationships among amino acids. Contact maps are small dense graphs. In average a graph may have 380 vertices. 
Since target graphs are dense, we extracted from them different types of pattern graphs (from dense to sparse) to vary the performance comparisons. Patterns were generated from the corresponding target graphs giving the number of desired edges. Dense patterns are constructed by forcing the number of vertices to be approximately equal to 25% of the number of edges. Semi-dense patterns have a number of vertices almost equal to 50% of the number of edges. For the sparse patterns the percentage of vertices is set to 90% and cycles avoid simple structures as paths. Each pattern tends to reach the desired percentage of vertices. For each density of patterns, we create seven groups of 10 random patterns having a number of edges equals to 4, 8, 16, 32, 64, 128 and 256. 

[Huehne R, Suehnel J: The Jena Library of Biological Macromolecules. Nature-precedings 2009.]
[Protein Data Bank]( http://www.rcsb.org/pdb/.) <br>
[Boghossian N, Kohlbacher O, Lenhof H: BALL: Biochemical Algorithms Library. In Proceeding of the 3rd workshop on algorithms engineering WAE 99 Lecture Notes in Computer Science, 1668, Springer, Berlin, London, UK, pp. 330-344, 1999.]
[Vehlow C, Stehr H, Winkelmann M, Duarte JM, Petzold L, Dinse J, Lappe M: CMView: Interactive contact map visualization and analysis. Bioinformatics 2011.]

### Graemlin
>synthetic PPI

This dataset contains 10 microbial networks (Campylobacter jejuni, Caulobacter crescentus, Helicobacter pylori 26695, Salmonella typhimurium LT2, Synechocystis PCC6803, Vibrio cholerae, Escherichia coli K12, Mycobacterium tuberculosis H37Rv, Streptococcus pneumoniae TIGR4, Streptomyces coelicolor ). The dataset is proposed with original unique labels, and varying the number of assigned random labeled from 32, 64, 128, 256, 512, 1024, to 2048.Labels are assigned using a uniform distribution. 
We create sets of 20 dense, semidense and sparse patterns for each pattern dimension (4, 8, 16, 32, 64, 128, to 256).

[Flannick J, Novak A, Srinivasan B, McAdams H, Batzoglou S: Graemlin: general and robust alignment of multiple large interaction networks. Genome research 2006, 16(9):1169.]

### PPI
> protein-protein,interaction networks

This dataset contains 10 networks describing the known and predicted protein interactions downloaded from STRING. We used the following organisms: Mus musculus, Saccaromyces cerevisiae, Caenorhabditis elegans, Drosophila melanogaster, Takifugu rubipres, Danio rerio, Xenopus tropicalis, Bos taurus, Rattus norvegicus, and Homo sapiens. They are large dense graphs. 
The original version of the dataset having unique node labels (protein ids) is also randomly relabeled with 32, 64, 128, 256, 512, 1024, and 2048 number of labes. Labels are assigned using a uniform distribution and a normal distribution (gaussian). 
We extracted from the target graphs sets of 20 dense, semidense and sparse patterns for each pattern dimension (the number of edges vary from 4, 8, 16, 32, 64, 128, to 256). 
[Szklarczyk D, Franceschini A, Kuhn M, Simonovic M, Roth A, Minguez P, Doerks T, Stark M, Muller J, Bork P, Jensen L, von Mering C: The STRING database in 2011: functional interaction networks of proteins, globally integrated and scored. Nucleic Acids Res. 2011, 39.]

### Sansone et al.
>synthetic dataset

The synthetic dataset distributed by Sansone et al. They are pairs of unlabeled graphs having sizes varying from 20 to 1000 vertices. The dataset contains the following kinds of graphs: Bounded Valence: (the number of edges per vertex varies from 3, 6, 9), Mesh( 2D, 3D and 4D, where 2,3,4 indicate the dimensionality of the meshes), and Random (edges are added according to a fixed probability; edges are independent and the probability distribution is uniform). The synthetic dataset is composed of pairs of (target and pattern) graphs. 
[Foggia P, Sansone C, Vento M: A Database of Graphs for Isomorphism and Sub-Graph Isomorphism Benchmarking. Proceedings of the 3rd IAPR TC-15 Workshop on Graph-based Representations in Pattern Recognition 2001.]
