# SCHDNA
# De novo assembly analysis software by SCH university


made by Song




Run genome & transcriptome analysis processing scripts. usage: SCHDNA.py [-h] [-d DIRECTORY] [-i INPUT INPUT] [-c CONFIG] [-s START_STEP] [-transcriptome] [-genome]

'-h', --help            show this help message and exit
  
'-d', '--directory', type=str, help='Base directory for input and output files.'

'-i', '--input', type=str, help='Paths to the raw input files.'

'-c', '--config', type=str, help='Path to the program configuration file.'

'-s', '--start-step', type=int, default=1, choices=[1, 2, 3, 4, 5, 6, 7]
choices help='Step to start the process from (default: 1; Trim: 1, ReadCheck: 2, Assembly: 3, Scaffold: 4, Prediction: 5, Estimation: 6, RepeatMasker: 7)'

'-transcriptome'        Run the transcriptome pipeline. SCHDNA [-h] [-transcriptome] [-d /path/to/base] [-i /path/to/raw_1.fq.gz /path/to/raw_2.fq.gz] [-c /path/config_file] [-s START_STEP]
'-genome'               Run the genome pipeline. SCHDNA [-h] [-genome] [-d /path/to/base] [-i /path/to/raw_1.fq.gz /path/to/raw_2.fq.gz] [-c /path/config_file] [-s START_STEP]

To use this program, you must prepare a configuration file.





## Making config.txt

# Transcriptome

TRINITY_PATH=/path/trinityrnaseq-v2.15.2/Trinity

TRANSD_PATH=/path/TransDecoder

TGICL_PATH=/path/TGICL-2.1/bin/tgicl


# Genome

TRIMMOMATIC_PATH=/path/Trimmomatic-0.36/trimmomatic-0.36.jar

ADAPTER_PATH=/path/Trimmomatic-0.36/adapters/TruSeq3-PE.fa

MEGAHIT_PATH=/path/MEGAHIT-1.2.9-Linux-x86_64-static/bin/megahit

SSPACE_PATH=/path/SSPACE-STANDARD-3.0_linux-x86_64/SSPACE_Standard_v3.0.pl

GAPFILLER_PATH=/path/SSPACE-STANDARD-3.0_linux-x86_64/GapFiller.pl



####################################################################

