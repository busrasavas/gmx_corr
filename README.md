# Conversion of covariance matrix to cross correlation matrix with gmx_corr

[![DOI](https://zenodo.org/badge/436035260.svg)](https://zenodo.org/badge/latestdoi/436035260) 

#### by A. Berçin Barlas, Büşra Savaş and Ezgi Karaca

## Motivation
Dynamic cross correlation analysis (DCCA) is commonly used for interpreting molecular dynamics simulations. Moreover, DCC is useful to analyze communications among different parts of complex systems. Despite the popularity of this analysis, we noticed that GROMACS does not directly provide the cross correlation matrix. Here, we introduce a simple script that converts the covariance matrix produced by GROMACS covar to cross correlation matrix and creates its heatmap.

**Usage Example(s)**

```
    #Load the output file of GROMACS covar ascii.
    covar = pd.read_csv(r'../application_example/covar-3a-cgc.dat', sep=' ', header=None)
    
    #Convert the covariance matrix to cross-correlation and save it to csv file.
    np.savetxt("../outputs/cross_corr_3a-cgc.csv", corr, delimiter=" ", fmt='%s')
    
    #Draw the graph and save it.
    fig.savefig('../outputs/cross_corr_3a-cgc.jpeg', dpi=500)
```
## Our folders describe:

- **input:** contains our test input files
- **outputs:** contains our test output files
- **jupyter-notebook:** contains the jupyter notebook script to convert covar matrix to a cross correlation matrix and its heatmap.
  

## Contact 
ezgi.karaca@ibg.edu.tr
