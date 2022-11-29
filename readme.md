Analysis of ribosome profiling data from HAP1 cells treated with 4-thiouracil & UV light to induce RNA-protein crosslinks

See: Translation-coupled sensing and degradation of RNA-protein crosslinks by Stingele et al

    Copyright (C) 2022 Allen Buskirk

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <https://www.gnu.org/licenses/>.


Developed by Allen Buskirk. Some code was originally written by Anthony Veltri. Address questions to buskirk@jhmi.edu

This code is provided to aid in understanding how the data were processed and analyzed in this study. No warranties are given as to its applicability outside of this study. 

Dependencies:

Jupyter notebook, python 3.9.7, STAR 2.7.10a, samtools 1.7, BBTools 38, and various python modules listed in the import statements (e.g. bokeh 2.4).

The raw sequencing data are available as FASTQ files at the GEO, accession number XXX.

Processing of the FASTQ files, mapping with STAR, and and storing ribosome density are all described in the iPython notebook read_processing. The metagenes notebook describes how the average ribosome density plots were generated. The conversions notebook describes how T to C conversions were counted from the aligned bam files.

A parsed GTF file (h38 ensemble) and transcript dataframe used in the analyses are provided as pickled dataframes. Also a parsed VCF file is provided as a pickled dataframe (bcf_df_pkl) revealing the differences of the HAP1 cells from the hg38 annotation (these were obtained from three replicates of untreated RNAseq).