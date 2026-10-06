# Project overview

This project aims to investigate wether it's possible to model the data presented in table 2 in (Llopart et al., 2025) according to a poisson distrubution and determine the accuracy of that model.

The program rendered values that were similar to the ones observed from the paper, which means that a possion distribution is a possible model for the data investigated. However, since the expected values generated from the model and the observed values from the article weren't a complete fit, a poisson distribution does not describe the biology behind the crossover events discussed in the paper. Additionally, since only a few chromosome arms are presented in the data, the model might not represent the reality of other chromosome arms.

## The paper

The article presents a genome-wide, high-resolution crossover map for the fruit fly Drosophila santomea and compares it to other closely related fruit flies. The researshers examined 784 individual meiotic products that captured intraspecific variation in crossing over control and identified 2,288 genome-wide crossovers. The findings suggested a link between the intensity of crossover interference and the centromere effect, and the researchers proposed that "stronger crossover interference is associated with a smaller crossover-competent region—determined by the combined

## Requirements

The project uses python and the following packages:

NumPy

Math

Matplotlib

## Usage

Open and run `project.ipynb`

The source data from *Table 2* of the paper is also provided in `data/Crossover_data.xlsx`

## Reference

Llopart, A., Pettie, N., Ryon, A. and Comeron, J.M. (2025). A high-resolution crossover landscape in Drosophila santomea reveals rapid and concerted evolution of multiple properties of crossing over control. PLOS Genetics, 21(10), p.e1011885. doi:10.1371/journal.pgen.1011885.


