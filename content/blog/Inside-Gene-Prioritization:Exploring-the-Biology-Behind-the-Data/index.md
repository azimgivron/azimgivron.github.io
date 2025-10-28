---
# Featured image
image:
  caption: "DNA"
title: "Inside Gene Prioritization: Exploring the Biology Behind the Data"
summary: "This article introduces the concept of gene prioritization in bioinformatics, explaining the biological principlesunderlying how genes influence life and disease, and outlining the main data sources used before addressing the computational perspective."
date: 2023-10-27

# Featured image
authors:
  - admin

tags:
  - Gene Prioritization
  - Genome
  - Exome
  - Genomics
  - Biology
  - Bioinformatics

# content_meta:
#   trending: true
---

{{< toc mobile_only=true is_open=true >}}

In this article, I discuss the problem of gene prioritization in bioinformatics. This topic was actually the subject of my second master’s thesis. My goal is to introduce the problem and discuss the biological foundations and data sources involved. We will focus first on the biological aspect, leaving the machine learning perspective for later.

To understand the problem of gene prioritization, we must first examine the fundamental role that genes play in life, disease, and death. Next, we will explore how biologists study the complex relationships between genes and biological processes. With this foundation, we will then be able to formally define the gene prioritization task and review the main data sources used to address it.

### When Genetic Information Goes Wrong: How Mutations Lead to Disease

Living organisms are made of cells, the smallest structural and functional units of life, capable of performing all essential biological processes. Each cell is enclosed by a membrane and contains a nucleus. Between the membrane and the nucleus lies the cytoplasm, which holds various organelles, specialized structures that perform distinct functions such as energy production, protein synthesis, and waste processing [4].

The nucleus contains the organism’s genetic material, organized into Deoxyribonucleic Acid (DNA). DNA stores the instructions required for the organism’s development, functioning, and reproduction. It is composed of sequences of nucleotides, each consisting of a phosphate group, a deoxyribose sugar, and one of four nitrogenous bases: adenine (A), thymine (T), cytosine (C), or guanine (G). The specific order of these bases encodes the information used to synthesize proteins, which are responsible for carrying out most cellular functions essential to life [3].

Proteins serve a wide range of roles within the cell. Enzymes act as catalysts that accelerate biochemical reactions fundamental to metabolism and energy production. Structural proteins, such as actin, tubulin, and collagen, maintain cell shape, enable movement, and form the framework of tissues. Transport proteins, including hemoglobin and membrane transporters, facilitate the movement of molecules like oxygen, ions, and nutrients within and between cells. Finally, regulatory proteins, such as transcription factors, control gene expression by determining when and how specific genes are activated or repressed, ensuring that each cell produces the right proteins at the right time [2].

Within the cell’s nucleus, DNA is not found as a loose, continuous strand. Instead, it exists in a double-helical structure that is tightly coiled and packaged into compact units called chromosomes. Each chromosome contains a long molecule of DNA wrapped around proteins known as histones, which help maintain its structure and regulate gene accessibility [3].

Further segmentation of this DNA reveals specific regions called genes, each encoding the information required to produce a particular protein that contributes to the cell’s structure, function, or regulation. However, genes are not continuous stretches of coding information, they are composed of exons and introns. Exons are the portions of a gene that contain the actual coding sequences used to synthesize proteins, while introns are non-coding regions that interrupt these sequences. Gene expression refer to the process of turning genetic information into something that works inside the cell. During gene expression, introns are removed through a process called RNA splicing, and exons are joined together to form a continuous sequence that can be translated into a functional protein [3].

When we are born, all our genetic information is contained in our DNA, which holds the complete set of instructions determining how our body is formed and functions at birth. However, the environment also influences our body over time, shaping its development, physiology, and overall health.  All humans begin life as a single cell, the fertilized egg, which then undergoes countless rounds of cell division to form the complex organism we become. Throughout our lives, cells continue to divide and renew, while others age and die. This constant cycle of cell death and renewal maintains our tissues and organs. For instance, when we sustain an injury, damaged tissues are repaired through the formation of new cells that replace those lost. But how does a cell know how to replicate itself? The answer lies within DNA, which serves as a biological cookbook containing all the instructions required for cell division. During this process, the DNA is duplicated so that each new cell receives an identical copy of the genetic information, ensuring the continuity of life and function across generations of cells [4].

Of course, if this “cookbook” becomes corrupted, for example, through a mutation in the DNA, and the damaged cell continues to survive and replicate, the number of corrupted cells can increase over time. If the body’s repair or control mechanisms fail to correct the error, and the mutation occurs in a critical region of the genome, that is, the entire set of an organism’s genetic material, such as one controlling cell growth or metabolism, it can ultimately lead to a genetic disease. A well-known example is cystic fibrosis, caused by mutations in the *CFTR* gene, which disrupts the production of a protein responsible for regulating salt and water balance in cells. This defect leads to the buildup of thick mucus in the lungs and digestive system, demonstrating how a single genetic error can have widespread physiological consequences. However, not all genetic mutations immediately result in disease. Many mutations are benign when occurring alone, as the cell can often compensate for minor changes. Yet, because proteins regulate numerous cellular processes, and cells themselves encode the information for synthesizing proteins, multiple small mutations can interact through molecular pathways, gradually disturbing the system’s balance. A molecular pathway is a series of interconnected biochemical reactions within a cell, where proteins and other molecules work together to carry out specific functions. Over time, this accumulation of seemingly harmless changes can lead to disease. A prominent example is cancer, where numerous minor mutations in genes involved in cell-cycle regulation, DNA repair, and signaling pathways together compromise normal growth control, ultimately driving uncontrolled cell proliferation and tumor formation. Moreover, a single gene may contribute to several disorders, and genes often interact in non-additive ways, either synergistically or antagonistically, to influence disease susceptibility. In this broader context, even modest genetic alterations can disrupt the intricate regulatory balance within cells, setting the stage for disease development [1].

In summary, humans are composed of cells that regulate their functions through protein synthesis, directed by the information encoded in DNA. When this genetic information is altered or corrupted, it can disrupt normal cellular regulation and lead to disease. In the following sections, we explore how scientists identify and relate specific genes to diseases, and why uncovering these associations is essential for advancing diagnosis, treatment, and biological understanding.


### Unraveling the Connection Between Genes and Disease: A Wet Lab Perspective

## Online Mendelian Inheritance in Man (OMIM)

OMIM \cite{OMIM} is a comprehensive, curated database that catalogs human genes and the phenotypes associated with them, with a particular focus on Mendelian (single-gene) disorders.

In genetics, the genotype refers to the specific genetic makeup of an organism, that is, the sequence of DNA that determines particular traits or predispositions. For example, carrying a mutation in the *BRCA1* gene represents a genotypic variation that increases susceptibility to breast and ovarian cancer. In contrast, the phenotype refers to the observable characteristics or traits that result from the interaction between the genotype and the environment. For instance, developing breast cancer due to the *BRCA1* mutation represents the phenotypic expression of that genetic variation.


1. Vogelstein, B., Papadopoulos, N., Velculescu, V. E., Zhou, S., Diaz Jr., L. A., & Kinzler, K. W. (2013). Cancer genome landscapes. *Science, 339*(6127), 1546–1558. [https://doi.org/10.1126/science.1235122](https://doi.org/10.1126/science.1235122)
2. Berg, J. M., Tymoczko, J. L., & Gatto, G. J. (2019). *Biochemistry* (9th ed.). New York: W. H. Freeman.
3. Watson, J. D., Baker, T. A., Bell, S. P., Gann, A., Levine, M., & Losick, R. (2013). *Molecular Biology of the Gene* (7th ed.). San Francisco: Pearson Education.
4. Alberts, B., Johnson, A., Lewis, J., Morgan, D., Raff, M., Roberts, K., & Walter, P. (2015). *Molecular Biology of the Cell* (6th ed.). New York: Garland Science.
