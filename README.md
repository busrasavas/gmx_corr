# Conversion of covariance matrix to cross correlation matrix with gmx_corr

THIS REPO IS UNDER DEVELOPMENT, please contact with ezgi.karaca@ibg.edu.tr before using!

#### by A. Berçin Barlas, Büşra Savaş and Ezgi Karaca

## Motivation
Dynamic cross correlation analysis (DCCA) is commonly used for interpreting molecular dynamics simulations. Moreover, DCCC is useful to analyze communications among different parts of complex systems. Despite the popularity of this analysis, we noticed that GROMACS does not directly give the relevant outputs. Here, we introduce a simple script that converts the covariance matrix produced by GROMACS covar to cross correlation matrix and creates a heat map figure.

**Quick Example(s)**

```
    #Load the output file of GROMACS covar ascii.
    covar = pd.read_csv(r'../application_example/covar-3a-cgc.dat', sep=' ', header=None)
    
    #Convert the covariance matrix to cross-correlation and save it to csv file.
    np.savetxt("../outputs/cross_corr_3a-cgc.csv", corr, delimiter=" ", fmt='%s')
    
    #Draw the graph and save it.
    fig.savefig('../outputs/cross_corr_3a-cgc.jpeg', dpi=500)
```
## Our folders describe:

- **inputs:** contains all the relevant input files to re-obtain our outputs.
- **jupyter-notebook:** contains the jupyter notebook script to convert matrices and to obtain cross correlation graph.
- **outputs:** contains the output files produced by jupyter notebook script.
  

## To clone the repository

```
git clone https://github.com/busrasavas/gmx_corr.git
```
or if you would like to get the content directly via wget:
```
wget https://github.com/busrasavas/gmx_corr/archive/master.zip
```

## Contact 
ezgi.karaca@ibg.edu.tr
