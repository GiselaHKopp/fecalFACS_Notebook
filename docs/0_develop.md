---
title: "Project summary"
output: html_notebook
---
# Project development



 
## General idea
In this project, we will assess the general applicability of the fecalFACS method. We submitted a medium money grant proposal to the CASCB on 13.04.2021. We received the positive answer of funding of our project (informally) on 08.06.2021. 

## Project overview
More than five decades ago, W. D. Hamilton formulated his seminal “rule” on why individuals cooperate: They increase their inclusive fitness (i.e. the number of shared genes passed to the next genera-tion) by promoting the survival or reproduction of close kin [@Hamilton1964-bw; @Hamilton1964-ne]. The idea of kin selection as a driving force for social interactions has since become a central paradigm in behavioural ecology and evolutionary biology with many studies supporting its predictions; but it is also essential to weigh kin selection against other potential drivers, such as reciprocal altruism or direct benefits [@Smith2014-dk]. 
Testing these hypotheses is only possible if relatedness between individuals can be determined, which has been a difficult endeavour in natural populations of difficult-to-sample taxa. Standard methods to generate genetic data rely on DNA of high quality and quantity, which can only be obtained from blood or tissue samples. Collecting these samples from dozens or hundreds of individu-als, as desirable for behavioural studies, is often not feasible or may be prohibited. The development of methods that can generate genetic data from non-invasively collected samples (e.g. faeces, hair, and urine) revolutionized the field of behavioural ecology (4). These methods have traditionally used genetic marker systems that only represent a very small fraction of the genome and are imprecise in resolving fine-scale relationship patterns, especially in wild animal groups (5). Thus, while being sufficient for basic population genetic studies or pedigree reconstructions in well-known study populations, the techniques for non-invasive genetic analysis often fail to provide enough detail and accu-racy in populations without background demographic data. Additionally, they require substantial initial investments in developing appropriate genetic markers for species lacking genomic data. 
With novel sequencing technologies (6), sequencing of whole genomes has become attainable, and with decreasing costs genomics has become applicable to wild populations (7). Unlocking popula-tion genomics for non-invasively collected samples would make it possible to gather high-resolution relatedness data on wild populations of non-model organisms and to include gene-specific information instead of genome-wide averages. Studies based on whole-genome data can also take ad-vantage of the most recent analytical tool developments and are more comparable across species. Hence, they would allow to elucidate how genotypic composition or functional genomic variation shape the collective behaviour of wild animal groups, research questions that have provided exciting results in laboratory experiments (8, 9) but are currently not feasible in most natural populations. 
Although becoming cheaper, genome sequencing is still very expensive, especially if a large number of individuals is to be sequenced (e.g. all individuals in replicated social groups). One solution is to sequence many individual whole genomes to low coverage (10, 11) and apply probabilistic models across all nucleotide positions to calculate genotype likelihoods instead of trying to guess the “true” genotype per site (12). A number of population genomic methods and analytical tools have now been developed to specifically estimate genomic relatedness from such shallow sequencing data (13–16). While they mainly targeted studies of ancient and prehistoric human remains, they also hold great promise for studies of natural animal populations, especially if samples can only be obtained non-invasively and the resulting DNA holds the same pitfalls as ancient DNA (aDNA), i.e. very low DNA quality and quantity as well as extreme levels of contamination (17).  
These advances have huge potential to study kin selection and collective behaviour in the wild, but to date have not widely been integrated in field studies. The hesitancy of the animal behaviour research community to adapt these new approaches can be attributed to the perceived high expertise in mo-lecular technologies and bioinformatics as well as the infrastructure required to successfully imple-ment these protocols, which is usually beyond the capacity of individual research groups. I contribut-ed to the development of one of these methods, which allows the reconstruction of pedigrees in wild animal populations (17). This method estimates relatedness from low coverage whole genome data and avoids sequencing high amounts of contaminant DNA (which can be above 99% in fecal sam-ples) by enriching target DNA with capture baits prior to sequencing. The shortcoming of this method is that it still requires one high quality DNA sample to generate species-specific RNA baits for cap-ture enrichment. This limitation is circumvented in the novel fecalFACS approach (18), which uses fluorescence-activated cell sorting to preselect target cells from which DNA is subsequently extract-ed and sequenced. 
In this project, we will test the fecalFACS method as a tool to study genomic relatedness networks that underlie social interaction networks in natural animal populations. Importantly, we aim to implement a low-threshold semiautomatic pipeline, in which researchers can analyse their samples for genomic relatedness with little prior expert knowledge in the applied methods.

We will use two primate and two bat species as study systems to investigate the broad-scale feasibility and accuracy of the fecalFACS method. One primate and one bat species will serve as “setup spe-cies” to establish the method, the remaining two species will serve as “verification species” to evalu-ate the generalizability of the established workflow. The study species are selected for three main reasons: First, both primates and bats live in complex societies with highly differentiated social rela-tionships, making them prominent study systems to investigate social interaction networks and the evolution of cooperative behaviours. However, while kin selection is invoked as a strong factor in shaping social relationships in many group-living primates (19), its role in bats appears much more ambiguous (20). This will give us the opportunity to investigate genomic relatedness networks in spe-cies with contrasting predictions: we predict that in the primate species, social interaction networks reflect genomic relatedness networks, whereas we predict to find no strong link for the bat species. Second, we need to consider the influence of diet on the tested method. A high proportion of mam-malian prey items in the diet of the study species would likely decrease the amount of target se-quencing reads, because we would expect that many of the selected cells from the flow cytometry step would not represent the target study species but the prey it consumed. While we therefore chose to not investigate carnivorous species, we chose species with different diets that permit us to evaluate whether faunal prey can potentially be analysed simultaneously to the genomic relatedness networks. This could make this method especially interesting for species with cooperative hunting, as it would allow us to determine the individuals that consumed the same prey during a given time win-dow, as expected for cooperative hunting, including in both target bat species. Third, we selected study populations where we have ongoing studies focusing on collective behaviour. For these popu-lations, social interaction data are already available, but relatedness data would be crucial to interpret evolutionary questions. The collection of fecal samples is highly feasible in a short-term time frame and project delay due to time-consuming issuing of necessary permissions or the Covid19 pandemic can be ruled out (“setup species”) or minimized (“verification species”). 

### Work plan
Study groups and sample collection: Faecal samples will be collected from at least 40 individuals for each of the four study species. Samples from the “primate setup species” Barbary macaques (*Macaca sylvanus*) will be collected at Affenberg Salem, Germany, where approx. 180 Barbary ma-caque live in three groups under semi-natural conditions in a 14.5 ha forest enclosure. Samples from the “primate verification species” Ugandan red colobus (*Piliocolobus tephrosceles*) will be collected by Urs Kalbitzer and his team at the long-term research project at Kanyawara in Kibale National Park, Uganda. During daily observational follows, a sample will be collected immediately after defecation by an identified individual. Samples from the “bat setup species”, the common noctule bat (*Nyctalus noctula*) will be collected by Dina Dechmann and her team at the MPI-AB study sites in the Konstanz region. Samples from the “bat verification species”, the Greater noctule bat (*Nyctalus lasiopterus*) will be collected by Dina Dechmann and her collaborators Carlos Ibanez and Javier Juste at the Estación Biológica de Doñana (CSIC) in Spain. Samples will be collected from roosts during regular monitor-ing visits and identities of all individuals within the roost will be recorded. All samples will be stored in 5ml RNAlater at ambient temperature until transport to the laboratory at the University of Konstanz. 

#### Behavioural data
Association and social interaction data will be contributed by the collaborators of the respective study species and used to construct social interaction networks using the igraph package (21) in R (22). For Barbary macaques, we will use data on group and matrilineal membership, male coalitions, and male-infant interactions. For red colobus, we will use data on group member-ship, proximity, and grooming interactions. For both noctule bat species, we will use roosting association data as well as telemetry/GPS tracking data of groups. 

#### FecalFACS and Sequencing
Target cells for sequencing will be isolated from the fecal samples on a BD FACSAria Fusion (BD Biosciences) flow cytometer at the Flow Cytometry Centre (FlowKon) at the University of Konstanz following the published fecalFACS protocol (18). We will implement slight modifications to increase the precision of the cell sorting, i.e. evaluate the combination of different stains to achieve more specific selection criteria for each species. The effectiveness of the cell sort-ing will be microscopically confirmed at the BioImaging Centre (BIC) at the University of Konstanz. 
DNA laboratory work will be conducted at the University of Konstanz with necessary precautions for the handling of fecal DNA. DNA will be extracted from the isolated cells using the Qiagen DNA Micro kit with modifications to increase DNA yield (18). Final DNA concentration will be measured with a Qubit fluorometer and quality checked on a TapeStation 2200. Whole-genome sequencing libraries will be prepared with the NEBNext Ultra II kit and 150bp paired-end sequenced on an Illumina No-vaSeq6000 at the Sequencing Core facility of the MPI Molecular Genetics in Berlin to achieve 1-2X coverage.  

#### Sequencing data processing and analyses
Sequence data will be processed and analysed with a modified version of our nextflow pipeline for genotype likelihood calling and relatedness estimation from shallow whole genome sequencing data (23), which we have developed in collaboration with the Sequencing Analysis Core Facility (SequAna) at the University of Konstanz. We will use the M. sylva-nus data set to evaluate the precision and accuracy of our analyses by comparing the obtained relat-edness coefficients to long-term monitoring data of the study population and known mother-offspring pairs (for which a relatedness coefficient of 0.5 is to be expected). For each species, we will build relatedness networks using relatedness coefficients as edge weights using igraph. To as-sess the correlation between social interaction networks and genomic relatedness networks we will use multilayer network methods (24) and (for each species) calculate edge overlap between the con-structed networks as implemented in MuxViz (25). 

## Project metadata

### Species
* Barbary macaque (*Macaca sylvanus*)  
* Ugandan red colobus (*Piliocolobus tephrosceles*)  
* common noctule bat (*Nyctalus noctula*)  
* Greater noctule bat (*Nyctalus lasiopterus*)

### Locations
Samples were collected in the following locations:  

* Affenberg Salem (Barbary macaque samples)  
  Salem, Germany  
  Contact: Dr. Roland Hilgartner (director)
  responsible: Gisela
  
* Kanyawara (red colobus)  
  Uganda  
  Kibale National Park   
  responsible: Urs
  
* Konstanz (common noctule)  
  Germany
  responsible: Dina
  
* Estacion Biologica de Donana (CSIC) (Greater noctule)
  Spain
  contact: Javier Juste
  responsible: Dina
  
### Dates
Samples were collected: 

* 05- 2021 (Barbary macaques, Affenberg Salem)
* 07/2021 (Greater noctule, Donana)

### People
**Gisela H. Kopp**
PI  
Sociality & Evolution/Zukunftskolleg & Dept. Biology, University of Konstanz  
gisela.kopp@uni-konstanz.de  
responsibilities: general project coordination, finances, sample collection Barbary macaques, laboratory analysis and supervision of research assistant, data analysis, manuscript writing

**Dina Dechmann**
collaborator  
Migration/MPI Animal Behaviour  
ddechmann@ab.mpg.de  
responsibilities: sample collection bats (incl. permits), bat behavioural data, manuscript writing  

**Urs Kalbitzer**
collaborator    
EAS/MPI Animal Behaviour  
ukalbitzer@ab.mpg.de  
responsibilities: sample collection colobus (incl. permits), colobus behavioural data, manuscript writing

**Camila Calderon**
collaborator  
Migration/MPI Animal Behaviour  
ccalderon@ab.mpg.de  
responsibilities: *Phyl.* sample collection (incl. permits)

**Melina Dietzer**
research assistant  
Sociality & Evolution/University of Konstanz  
melina.dietzer@ab.mpg.de  
responsibilities: laboratory analysis, sample & data management

### Permits
!!!!!!!!! Permit name, granting organization, permit number

### Funding
Project funding via CASCB Medium money grant 2021. GHK funded by Hector Pioneer Fellowship (Hector Foundation II & University of Konstanz). DD ???. UK ???. CC ???. 

### Data storage


---
