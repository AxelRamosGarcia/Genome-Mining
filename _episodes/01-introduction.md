---
title: "Introduction to Genome Mining"
teaching: 10
exercises: 0
questions:
- "What is Genome Mining?"
objectives:
- "Understand that Natural products are encoded in Biosynthetic Gene Clusters."
- "Understand that Biosynthetic Gene Clusters can be identified in the genomic material."
- "Discuss bioinformatic's good practices with you colleagues."

keypoints:
- "Natural products are encoded in Biosynthetic Gene Clusters"
---

## Genome mining aims to find BGCs

Natural products are encoded in a Biosynthtetic Gene Clusters (BGCs) in Bacteria. These BGCs are clusters of genes that are placed together in the same genome region. These includes, not only those genes encoding the biosynthetic enzymes, but also those related with the transport of the metabolite or with the resistance against antibacterial metabolites.
Genome mining is the action of analyze genomes with specialized algorithms 
designed to find some BGCs. Some of these clusters were dilligently characterized 
by chemists last century. Right now we have extensive databases that contain
information about which genes belong to which BGCs, and some control sets of genes that does not. The use of genome mining methodologies facilitates the prioritization of BGCs for the search of novel metabolites.
Since the era of the next generation sequencing, genomes have been explored 
as a source for discovering new BGCs.

## Chloramphenicol is a known antibiotic produced in a BGC

As an example, let's have a look into the BGC responsible of the chloramphenicol biosynthesis. This is a BGC described for first time in a _Streptomyces venezuelae_ genome.
<a href="{{ page.root }}/fig/episode1-fig1.PNG">
  <img src="{{ page.root }}/fig/episode1-fig1.PNG" alt="" />
</a>
[Explore the BGC](https://mibig.secondarymetabolites.org/repository/BGC0000893/index.html#r1c1)

## Planning a genome mining project  
Here we will provide tips and tricks to do plan and execute a genome minning project. Let's start!
First, a set of genomes from taxa should be chosen. In this lesson
we will be working with _S. agalactiae_ genomes (Tettelin et al., 2005) (https://zenodo.org/record/6595388#.YtD9LsFBxUJ). This genus is not know
for its capabilities as a Natural products producer but is good enough
to show different approaches to genome mining. Recently, metagenomes have been 
considered in genome mining studies. Here are some considerations 
that may be useful for you as a genome miner: 

- Think about your research questions before start analyzing the data.  
- Remember, raw metadata should remain intact during all genome mining process.
It could be a good idea to change its file-permisions to read only.    
- Gather as much information in the form of metadata of 
all the genomes that you are working with.  
- All your intermediate steps should be considered temporal 
 and maybe removed without risk.   
- Save your scripts using a version manager, GitHub for example.
- Share your data in public repositories.   
- Give time to make your science repeatable, help your community.    

## Starting a genome mining project
Once that you have choosen your set of genomes, you need to annotate the sequences. The process of genome annotation needs two steps. First, a gene callling approach (structural annotation), which looks for CDS or RNAs within the DNA sequences. Once these features have been detected, you need to assign a function for each CDS (functional annotation). This is usually done through the comparison against protein databases. There are tens of bioinformatic tools to annotate genomes, but some of the most broadly used ones are RAST (Aziz et al. 2008), and Prokka (Seeman, 2014). Here, we will start the genome minning lesson with  _S. agalactiae_ genomes already annotated by RAST. You can download this data from this [repository](https://zenodo.org/record/6595388#.YtD9LsFBxUJ). The annotated genomes are written in GeneBank format (extension ".gbk"). These files are also accesible in the... **Insert introduction related to the access to the server??**

## References
- Aziz, R. K., Bartels, D., Best, A. A., DeJongh, M., Disz, T., Edwards, R. A., ... & Zagnitko, O. (2008). The RAST Server: rapid annotations using subsystems technology. BMC genomics, 9(1), 1-15.
- Seemann, T. (2014). Prokka: rapid prokaryotic genome annotation. Bioinformatics, 30(14), 2068-2069.
- Tettelin, H., Masignani, V., Cieslewicz, M. J., Donati, C., Medini, D., Ward, N. L., ... & Fraser, C. M. (2005). Genome analysis of multiple pathogenic isolates of Streptococcus agalactiae: implications for the microbial ???pan-genome???. Proceedings of the National Academy of Sciences, 102(39), 13950-13955.

{% include links.md %}

