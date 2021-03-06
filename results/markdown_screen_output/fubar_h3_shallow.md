
Analysis Description
--------------------
Perform a Fast Unbiased AppRoximate Bayesian (FUBAR) analysis of a
coding sequence alignment to determine whether some sites have been
subject to pervasive purifying or diversifying selection. Please note
that a FUBAR analysis generates a cache and a results JSON file in the
same directory as directory as the original alignment. HyPhy needs to
have write privileges to this directory. For example if the original
file is in /home/sergei/FUBAR/data/pol.nex then at the end of a FUBAR
run, there will also exist FUBAR-generated files
/home/sergei/FUBAR/data/pol.nex.fubar.json,
/home/sergei/FUBAR/data/pol.nex.fubrarcache. They also provide
checkpointing so that a partially completed analysis can be restarted.

- __Requirements__: in-frame codon alignment (possibly partitioned) and a phylogenetic tree
(one per partition)

- __Citation__: FUBAR: a fast, unconstrained bayesian approximation for inferring
selection (2013), Mol Biol Evol. 30(5):1196-205

- __Written by__: Sergei L Kosakovsky Pond

- __Contact Information__: spond@temple.edu

- __Analysis Version__: 2.0



>A tree was found in the data file: `(KF790049:0.001255,((((((((CY134956:0.000624,CY183153:0.000624):0.0,(CY186123:0.000624,CY186051:0.000624):0.0):0.0,(((CY182809:0.000624,(((CY148436:0.0,CY168583:0.000624):0.0,CY170911:0.000624):0.0,KF789547:0.00125):0.000624):0.0,(CY186019:0.000625,(CY182889:0.000624,CY135132:0.0):0.00125):0.000624):0.0,((CY170799:0.001249,CY149260:0.000624):0.0,((CY134686:0.0,(CY168887:0.000625,KF790064:0.001249):0.0):0.000625,CY169023:0.000625):0.000624):0.0):0.0):0.0,((((CY183049:0.000624,((KF789535:0.001876,CY134740:0.000624):0.0,KF790356:0.000624):0.0):0.0,(((((CY182737:0.000624,(CY168663:0.001879,KF789752:0.001253):0.000623):0.0,(CY186059:0.000624,CY183193:0.001249):0.000625):0.0,CY141264:0.000624):0.0,CY183113:0.000624):0.0,(((CY183241:0.000624,((((CY134828:0.0,KF199858:0.000625):0.0,(CY135124:0.000624,(CY134780:0.000624,CY168871:0.001249):0.0):0.0):0.0,CY135060:0.000624):0.0,KF789614:0.000624):0.0):0.000624,CY183033:0.000626):0.0,(CY168599:0.001249,(CY168063:0.0,(CY148364:0.000624,CY148596:0.000624):0.0):0.0):0.001248):0.0):0.0):0.0,CY134844:0.0):0.0,CY182865:0.000624):0.0):0.0,CY183185:0.000624):0.0,((((((CY186035:0.001249,CY183081:0.000624):0.0,CY135044:0.000624):0.0,KF789780:0.0):0.0,CY182793:0.000624):0.000624,((CY186235:0.002501,(CY134788:0.0,((((((CY170479:0.001265,KF790106:0.0):0.000624,CY141230:0.000624):0.0,(CY149084:0.0,CY169199:0.001249):0.001249):0.0,(KF789618:0.000624,CY141176:0.00125):0.0):0.0,(KF790361:0.000624,(CY141213:0.000625,(CY170647:0.000624,((((KF790316:0.000625,CY169535:0.000624):0.000624,CY170967:0.000624):0.0,(CY169527:0.000624,CY148348:0.0):0.000624):0.0,(CY168759:0.000624,CY170767:0.0):0.0):0.0):0.000624):0.0):0.0):0.0,CY141280:0.000625):0.000624):0.000625):0.0,CY182777:0.000623):0.0):0.0,((KF790448:0.000624,(CY183225:0.000625,CY134764:0.0):0.0):0.000624,(((KF790345:0.000624,(((CY182945:0.000624,CY186075:0.0):0.0,(KF790011:0.0,CY147297:0.000624):0.001249):0.0,(KF886358:0.001249,KF789871:0.003135):0.0):0.0):0.000624,((((KF790286:0.001248,(CY170991:0.0,CY171303:0.000624):0.0):0.00125,(KF886340:0.001879,CY147295:0.000627):0.001255):0.0,(CY168295:0.001256,(CY183177:0.001878,CY170543:0.000625):0.000626):0.000623):0.0,(((CY170719:0.001249,KF789613:0.001249):0.0,KF886303:0.000624):0.0,((KF886305:0.000624,(KF199854:0.001249,CY169807:0.001249):0.0):0.0,((KF790378:0.000624,(CY170823:0.001249,(CY170879:0.000624,CY170591:0.000624):0.0):0.001875):0.0,KF789701:0.000624):0.0):0.0):0.0):0.0):0.0,((CY171119:0.0,CY171199:0.00125):0.000624,(((((CY171631:0.001249,CY171407:0.000624):0.0,CY171639:0.00125):0.0,CY171055:0.000624):0.0,CY171351:0.000625):0.0,((CY141252:0.001876,(CY171583:0.000625,CY171231:0.000624):0.0):0.0,KF789998:0.0):0.0):0.0):0.001249):0.000624):0.0):0.0):0.0,(((KF790167:0.0,KF789569:0.000624):0.000624,(KF789714:0.000623,(CY134812:0.0,CY141279:0.000625):0.0):0.000624):0.0,(KF886357:0.000625,(CY171335:0.000624,CY171071:0.0):0.001877):0.001252):0.0):0.0,CY186027:0.000624):0.000626)`

>Would you like to use it (y/n)? Y


>Loaded a multiple sequence alignment with **121** sequences, **566** codons, and **1** partitions from `/home/sjspielman/evogenomics_hyphy/datasets/h3_shallow.fna`
> FUBAR will write cache and result files to _/home/sjspielman/evogenomics_hyphy/datasets/h3_shallow.fna.cache_ and _/home/sjspielman/evogenomics_hyphy/datasets/h3_shallow.fna.json_, respectively 


> Number of grid points per dimension (total number is D^2) (permissible range = [5,50], default value = 20, integer): 20
> Number of MCMC chains to run (permissible range = [2,20], default value = 5, integer): 5
> The length of each chain (permissible range = [500000,50000000], default value = 2000000, integer): 2000000
> Use this many samples as burn-in (permissible range = [100000,1900000], default value = 1000000, integer): 1000000
> How many samples should be drawn from each chain (permissible range = [50,1000000], default value = 100, integer): 100
> The concentration parameter of the Dirichlet prior (permissible range = [0.001,1], default value = 0.5): 0.5


### Obtaining branch lengths and nucleotide substitution biases under the nucleotide GTR model
* Log(L) = -3884.95, AIC-c =  8264.49 (247 estimated parameters)
* Tree length (expected substitutions/site) for partition 1 :    0.109

### Computing the phylogenetic likelihood function on the grid 
* Determining appropriate tree scaling based on the best score from a  20 x 20 rate grid
* Best scaling achieved for 
	* synonymous rate =  2.815
	* non-synonymous rate =  0.500
* Computing conditional site likelihoods on a 20 x 20 rate grid

### Running MCMC chains to obtain a posterior sample of (synonymous,non-synonymous) rate weights
* Using the following settings
	* Number of chains : 5
	* Steps/chain      : 2000000
	* Burn-in steps    : 1000000
	* Samples/chain    : 100
	* Dirichlet alpha  : 0.5
* Running MCMC chain 1
* Running MCMC chain 2
* Running MCMC chain 3
* Running MCMC chain 4
* Running MCMC chain 5

### Tabulating site-level results
|     Codon      |   Partition    |     alpha      |      beta      |     N.eff      |Posterior prob for positive selection|
|:--------------:|:--------------:|:--------------:|:--------------:|:--------------:|:-----------------------------------:|
|       19       |       1        |        0.965   |       11.116   |      262.733   |       Pos. posterior = 0.9520       |
|       49       |       1        |        0.910   |       16.020   |      326.820   |       Pos. posterior = 0.9745       |
|      241       |       1        |        1.075   |       23.292   |      335.621   |       Pos. posterior = 0.9901       |
----
## FUBAR inferred 3 sites subject to diversifying positive selection at posterior probability >= 0.9
Of these,  0.08 are expected to be false positives (95% confidence interval of 0-1 )
