# CB2330_Project

**The paper:** Llopart, A., Pettie, N., Ryon, E. and Comeron, J. M. (2025) The crossover landscape and interference in Drosophila santomea. PLoS Genetics 21:e1011885. https://doi.org/10.1371/journal.pgen.1011885

**The data object:** The data used in this project was based on table 2 in the article, which shows the number of crossovers for five different chromosome types and the total number of crossovers for five different types of chromosome arms. Thie different crossoncers are NCO, meaning no or zero crossovers, 1CO, meaning one crossover, 2CO for two crossovers, 3CO for three crossovers and 4CO for four crossovers. The types chromosome arms are 2L, 2R^2, 3L, 3R and X.

**The random variable chosen:** The variable analysed in this notebook was the number of crossover events occuring on a chromosome arm in a randomly selected meiotic product, for each type of crossover.

**What the paper does:** The article presents a genome-wide, high-resolution crossover map for the fruit fly Drosophila santomea and compares it to other closely related fruit flies. The researshers examined 784 individual meiotic products that captured intraspecific variation in crossing over control and identified 2,288 genome-wide crossovers. The findings suggested a link between the intensity of crossover interference and the centromere effect, and the researchers proposed that "stronger crossover interference is associated with a smaller crossover-competent region—determined by the combined centromere and telomere effects—to prevent the deleterious consequences of multiple crossovers occurring too close together".

**The generative model proposed:** A poission distribution was proposed as a mechanism for how the crossovers accumulates. The mechanism is choosen based on the fact that the data is based on a set number of crossover event and measures the number of crossovers for each event, for each type of crossover.

**Parameters and assumptions:** The parameter Theta was used to describe the average number of crossovers per crossover event. The crossover classes and the chromosomes mentioned under "The data object", as well as the number of crossovers happening per crossover event, for each type of chromosome.

**The forward simulation:** The forward simulation was produced by estimating theta as the number of crossovers divided by the number of meiotic events.

**The parameterization/fitting:** The estimated parameter Theta was fitted to the papers data by running a negative likelihood for the poisson distribution of theta and the total number of observed crossover event (denoted as counts) for each type of crossover (denoted as crossover_classes). The total number of observed crossover events were calculated as the sum of all five types of chromosome arms. The parameterization resulted in the fitted Theta value for each type chromosome arm.

**What/if the model adds to the paper:**

**Model limitations/how it breaks:** 
