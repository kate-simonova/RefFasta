# RefFASTA (reformat FASTA)

RefFasta is a toolkit used for processing sequence files. This tool can be used for reformatting nucleic acids and amino acids into FASTA format (reformatDNA, reformatAA). Some functions also used for generating some statistics about the sequence content (statistic_DNA, statistic_AA), as well as for generating subsequences (with get_region function) and translating sequence from nucleic acids to amino acids.

## Installation

Use the following commands in order to download all scripts and run scripts from every folder of your device.

```bash
git clone https://github.com/kate-simonova/refFasta.git
mv scripts/* -t /usr/local/bin
```

The alternative way to execute refFasta from any folder is to add this folder into your PATH variable, but this way would work only for your currently opened terminal window.

```bash
export PATH=$PATH:path/to/current/folder
```

If you sure that you will need to use this program frequently, please edit your .bash_profile or .bashrc adding path to this folder into variable $PATH.


The recommended version of Python is 3.5 and higher.

## Usage

By calling help option you will see the list of avaliable commands:

```bash

RefFasta is a toolkit for processing files into FASTA format

Usage: refFasta <command> <input> or cat <input> | refFasta <command>
Example: refFasta reformatDNA my_sequence.txt or cat my_sequence.txt | refFasta reformatDNA
Version: 0.1
Contact: Ekaterina Simonova <simonove@vscht.cz>

Options:
	-h|--help 		print detailed description of tool and its options

Commands:
	reformatAA 		 to reformate an amino acid sequence into FASTA format
	reformatDNA 		 to reformate an DNA sequence into FASTA format
	statisticAA 		 to get the basic statistics about the amino acid sequence
	statisticDNA 		 to get the basic statistics about DNA sequence
	reverse_complement 	 to create reverse complement strand of your DNA sequence
	get_region 		 to subsample a defined range from a DNA sequence
	translate 		 to translate your DNA sequence into protein

```
## Some useful notes

While running command below, please press Ctrl + D in order to stop python wainting for the input. 

```bash
refFasta get_region int1 int2 <input>
```

## Contributing

For major changes, please open an issue first to discuss what you would like to change.
