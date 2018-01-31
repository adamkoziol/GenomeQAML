[![Build status](https://travis-ci.org/OLC-LOC-Bioinformatics/GenomeQAML.svg?master)](https://travis-ci.org/OLC-LOC-Bioinformatics)
# GenomeQAML: Genome Quality Assesment with Machine Learning

The GenomeQAML is a script that uses a pre-computed ExtraTreesClassifier model in order to 
classify FASTA-formatted _de novo_ assemblies as bad, good, or very good. It's easy to use,
and has minimal dependencies.

## External Dependencies

- [Mash (v2.0 or greater)](https://github.com/marbl/mash)
- [Prodigal (>=2.6.2)](https://github.com/hyattpd/Prodigal)

Both of these need to be downloaded and included on your $PATH.

## Installation

All you need to do is install with pip: `pip install genomeqaml`. 

Usage of a virtualenv
is highly recommended.

## Usage

GenomeQAML takes a directory containing uncompressed fasta files as input - these will be classified and
the results printed to your screen.

To run, type `classify.py -t /path/to/fasta/folder`