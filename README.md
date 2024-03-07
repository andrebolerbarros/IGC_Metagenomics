# Pipeline for Shotgun Metagenomics @IGC 

The pipeline here presented is based on the one from fdcerqueira (https://github.com/fdcerqueira/Metagenomics/tree/main). 

Metagenomics workflow made as a part of an experiment designed to study the tempo and mode of adaptation of a new strain of *E. coli*, and other species present in the gut of obese mice. Those mice were leptin deficient mice and were colonized with a strain of *E. coli*. In addition to the invader strain, the mice were also colonized with another *E. coli* strain which typically resides in their normal gut microbiota.

The aim of the workflow is to process the metagenomics data and detect SNVs in metagenomic assembled genomes (MAGs).

This pipeline is divided into 4 main scripts that can be used by the user, with the ability of changing some specific parameters:
- **Assembly.sh**: performs pre-processing of fastq files, remove host contamination, and performs the assembly with respective assessment using
- **Binning.sh**: performs binning and taxonomy attribution.
- **instrain.sh**: performs all the steps for `inStrain`, including pre- and post-processing
- **Midas.sh**: uses `MIDAS`, with all the steps involved.



**Third party softwares used:**

megahit:
https://academic.oup.com/bioinformatics/article/31/10/1674/177884?login=true

NonPareil:
https://academic.oup.com/bioinformatics/article/30/5/629/246142?login=false

bbmap:
https://jgi.doe.gov/data-and-tools/software-tools/bbtools/

bowtie2:
https://www.nature.com/articles/nmeth.1923

SqueezeMeta:
https://www.frontiersin.org/articles/10.3389/fmicb.2018.03349/full

inStrain:
https://www.nature.com/articles/s41587-020-00797-0

dRep:
https://www.nature.com/articles/ismej2017126

sekit:
https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0163962

prokka:
https://academic.oup.com/bioinformatics/article/30/14/2068/2390517

prodigal:
https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-11-119
