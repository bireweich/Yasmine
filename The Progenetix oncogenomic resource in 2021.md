# Introduction
Progenetix is a publicly accessible cancer genome data resource (progenetix.org) 

It aims to provide a comprehensive representation of genomic variation profiles in cancer, through:
 - providing sample-specific CNA profiles and associated metadata
 - services related to data annotation, meta-analysis and visualization
  
It uses data from:
  - molecular cytogenetics (CGH, genomic arrays)
  - sequencing (whole-genome or whole- exome sequencing—WGS or WES)
  
 # Data expansion and new features
 ## Genomic profiling data
 where does the data come from
 
 ## Data processing update
 Our current model treats the most prevalent copy number as the baseline and derives the rel- ative copy number gain and loss per sample based on the assumption that the relative gene dosage imbalance exerts pathophysiological effects in cancer biology.
 
 ## Allele-specific copy number variation
 For the subset of SNP-array-based experiments—where the status of both alleles can be evaluated separately—
 
 loss of heterozygosity (LOH) profiles
 
# What is CNV/CNA?
Copy number aberrations (CNA) represent a type of nearly ubiquitous and frequently extensive structural genome variations. They are present in the majority of cancer types and exert functional impact in cancer development.
copy number variation 

# How will you describe or introduce progenetix (scale, data source, cancer types and so on)?
Progenetix is a publicly accessible cancer genome data resource.
It aims to provide a comprehensive representation of genomic variation profiles in cancer, through:
  - providing sample-specific CNA profiles and associated metadata
  - services related to data annotation, meta-analysis and visualization
  
Its data comes from:
  - molecular cytogenetics (CGH, genomic arrays)
  - sequencing (whole-genome or whole- exome sequencing—WGS or WES)

# Describe NCIt, ICOD, UBERON codes, and their relationships.
**NCI Thesaurus (NCIt)** provides reference terminology for many NCI and other systems. It covers vocabulary for clinical care, translational and basic research, and public information and administrative activities. 
It is is a widely recognized standard for biomedical coding and reference, used by a broad variety of public and private partners both    nationally and internationally

The **ICD-O topography system** provides organ- and substructure-specific mapping rooted in traditional clinical and diagnostic aspects of a ‘tumor entity’.

**UBERON** is a cross-species anatomical structural ontology system closely aligned with developmental processes.

# What are CNV segmentations and CNV frequencies, and how to use them? What are APIs and how to use APIs in progenetix?
Sadly, I could not find information on CNV segmentations or CNV frequencies.

An **application programming interface (API)** is a way for two or more computer programs to communicate with each other. It is a type of software interface, offering a service to other pieces of software. Progenetix is built with the intention of implementing the GA4GH Beacon API, which would lead to an extension of the resource’s features as well as adoption and promotion of emerging open data standards

# How does progenetix visualise CNA profiles?
<img width="963" alt="Screen Shot 2022-09-21 at 15 47 01" src="https://user-images.githubusercontent.com/114007953/191521121-3d6d1b99-3a2e-4bbf-8c4f-51c44ebc4b5e.png">

The top panel of the result page shows a summary with the number of matched samples, variants, calls and the frequency of alleles containing the CNA. The ‘Phenopackets’ link returns a json document of biosam- ples with the phenopacket-formatted response. The ‘UCSC region’ links externally to a University of California Santa Cruz (UCSC) browser track providing an overview of the genomic elements which map to the region of the observed variants. Also, customized visualization is enabled in the linked page ‘visualization options’, e.g. for selected chromosomal regions and grouping by subsets or studies. The lower panel is organized in four sections: (i) the ‘Result’ tab shows the genome-wide CNA by the percentage of samples with yellow (+) as CN gain and blue (−) as CN loss. Below the CNA plot is a table showing the list of sub- sets as defined by ICD-O-3 and NCIt Ontology terms sorted by frequency of matched samples within that subset. (ii) the ‘Biosamples’ tab shows information of matched biosamples, i.e. description, classifications and external iden- tifiers. The table can be downloaded in json or csv format. The further detail of the biosample can be accessed by clicking the biosample id. (iii) The ‘Biosamples Map’ tab shows a world map with the matched geological locations highlighted. (iv) the ‘Variants’ tab shows the variant ‘digest’ (concatenated format with chromosome, start and end position, and type of the CNA) and its corresponding biosample and callset. Likewise, the table can be downloaded in json or csv format.

# What do you think should be improved in progenetix?
