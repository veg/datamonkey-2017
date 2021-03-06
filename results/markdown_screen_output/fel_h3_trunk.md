
Analysis Description
--------------------
FEL (Fixed Effects Likelihood) estimates site-wise synonymous (&alpha;)
and non-synonymous (&beta;) rates, and uses a likelihood ratio test to
determine if beta &neq; alpha at a site. The estimates aggregate
information over all branches, so the signal is derived from pervasive
diversification or conservation. A subset of branches can be selected
for testing as well, in which case an additional (nuisance) parameter
will be inferred -- the non-synonymous rate on branches NOT selected for
testing. Multiple partitions within a NEXUS file are also supported for
recombination - aware analysis. 

- __Requirements__: in-frame codon alignment and a phylogenetic tree

- __Citation__: Not So Different After All: A Comparison of Methods for Detecting Amino
Acid Sites Under Selection (2005). _Mol Biol Evol_ 22 (5): 1208-1222

- __Written by__: Sergei L Kosakovsky Pond and Simon DW Frost

- __Contact Information__: spond@temple.edu

- __Analysis Version__: 2.00


> A tree was found in the data file: `((KF790010:0.001247,CY147300:0.000623):0.0,((CY168239:0.001872,(CY171039:0.001874,KF790389:0.000623):0.000624):0.0,((CY141224:0.001247,(CY147305:0.0,KF790037:0.000623):0.000623):0.0,(((KF790403:0.000623,KF761507:0.001876):0.0,KC526205:0.000623):0.0,((CY169303:0.0,(KF789585:0.000623,CY141202:0.000623):0.000623):0.000623,(((KJ667974:0.002501,KJ938675:0.001873):0.000623,CY134876:0.0):0.000623,((KF790414:0.001248,(KF790384:0.001245,KF790408:0.00125):0.0):0.0,((KF886352:0.001882,(KF790438:0.000623,CY134996:0.001873):0.000623):0.001875,(KF789591:0.001879,((KF790049:0.001255,(CY134956:0.000624,CY183153:0.000624):0.000626):0.001249,((CY168407:0.004394,CY183065:0.003128):0.0,(KF598733:0.002501,((KC892174:0.0,(KF685747:0.000624,CY168471:0.000625):0.00375):0.000624,(((KC892685:0.000624,KC892641:0.0):0.001874,KC893110:0.001249):0.0,(KC892480:0.0,(JX913043:0.001249,(KF551075:0.00125,((CY114509:0.0,(KC892889:0.0,KC893018:0.002498):0.005006):0.001877,(((KC892519:0.0,KC892498:0.000624):0.002497,KC892266:0.000623):0.001026,((KC892156:0.003756,(JX978746:0.001256,KC892407:0.001883):0.001875):0.00355,((KC535402:0.000623,(KC882488:0.002498,KC535387:0.001247):0.001872):0.0,(KC535363:0.000623,((KC535396:0.000623,(KC882883:0.0,KC882867:0.000623):0.003124):0.0,((KC535378:0.001872,KC535375:0.002498):0.0,(GQ385891:0.001248,((EU779522:0.001251,(CY037727:0.0,FJ179354:0.003124):0.0):0.000623,((GQ385889:0.005007,(FJ686933:0.001243,FJ179356:0.003117):0.0):0.000622,(CY173095:0.001245,(((CY173191:0.0,CY037703:0.001247):0.000622,CY035062:0.00249):0.0,((CY173255:0.001871,(CY044748:0.0,GQ385846:0.001247):0.000623):0.0,((CY027075:0.000623,(EU199367:0.0,CY172823:0.000623):0.0):0.000623,(((CY172847:0.000623,CY025643:0.0):0.000623,CY172839:0.000623):0.001247,(((CY026251:0.002497,CY092241:0.00125):0.000624,CY026019:0.000623):0.0,((CY025341:0.002502,(CY172775:0.001247,CY172903:0.000623):0.001248):0.000622,(EU199255:0.003134,(CY172431:0.000621,((CY172223:0.003127,(CY172191:0.001254,CY020069:0.000628):0.000621):0.0,((CY092217:0.003119,(CY025485:0.001283,EU516019:0.00059):0.008843):0.001868,(CY002080:0.000622,((CY002064:0.001873,(CY002456:0.000626,CY002048:0.002491):0.001243):0.003763,(AB434109:0.006307,(((CY088198:0.001245,CY088475:0.000621):0.0,CY000257:0.000621):0.002494,((CY112957:0.003135,CY006859:0.001253):0.000616,((CY000721:0.001243,(CY114493:0.0,CY090885:0.002483):0.002488):0.0,((CY001792:0.000621,(CY001600:0.00062,CY002368:0.001865):0.0):0.0,((CY002304:0.002489,(CY006163:0.001242,CY003632:0.00062):0.0):0.00062,(CY001920:0.003739,(CY001912:0.002498,((CY001504:0.0,CY006060:0.001241):0.00062,((CY001744:0.0,CY002136:0.00124):0.00062,((CY114309:0.003746,(CY006899:0.001874,CY112901:0.001863):0.002496):0.000618,(((CY006579:0.001245,CY006283:0.000621):0.001244,CY007979:0.001864):0.0,((CY006499:0.001241,(CY006491:0.001863,CY006635:0.00124):0.0):0.00062,(((CY036847:0.002495,CY010004:0.001867):0.000621,CY012200:0.000621):0.0,(((CY010028:0.001242,CY009732:0.001242):0.0,CY010012:0.002484):0.001875,(((CY010020:0.002497,CY011416:0.001237):0.001252,CY009484:0.00062):0.005658,((CY010036:0.0,(CY039879:0.002489,CY039880:0.000621):0.002487):0.003109,((CY010628:0.000619,(CY010716:0.002485,CY010516:0.001239):0.0):0.000619,((CY012728:0.0,CY013701:0.000621):0.001243,(((CY012760:0.001239,CY013200:0.001239):0.0,CY011888:0.005614):0.0,((CY013693:0.000619,(CY012184:0.002484,CY013669:0.00124):0.00124):0.0,((CY112669:0.004353,(CY112556:0.001861,CY011896:0.000619):0.00186):0.0,(CY112605:0.001243,(CY012224:0.006953,((CY012512:0.000619,(CY012896:0.00062,CY012232:0.00062):0.000621):0.0,(CY011848:0.0,(((CY011328:0.0,CY114221:0.000619):0.001241,CY011560:0.00124):0.0,((CY012456:0.000619,CY011824:0.00124):0.0,CY017283:0.000619):0.0):0.0):0.0):0.002439):0.008263):0.000618):0.0):0.0):0.000617):0.012609):0.000619):0.001215):0.003782):0.000613):0.006878):0.0):0.001862):0.0):0.0):0.001863):0.001862):0.001245):0.0):0.001241):0.021084):0.000623):0.00065):0.003713):0.002495):0.0):0.005637):0.00313):0.002515):0.001876):0.0):0.000623):0.0):0.003749):0.0):0.0):0.000623):0.000623):0.001872):0.002503):0.0):0.0):0.000623):0.001468):0.00189):0.002721):0.002524):0.0):0.000624):0.0):0.0):0.0):0.000623):0.001248):0.001255):0.000619):0.0):0.0):0.0):0.000623):0.0):0.0):0.0)`
>Would you like to use it? Y


>Loaded a multiple sequence alignment with **163** sequences, **566** codons, and **1** partitions from `/Users/sjspielman/Research/book-chapter-2017/datasets/trunk.dat`
Yes

>Select the p-value used to for perform the test at (permissible range = [0,1], default value = 0.1): 0.1


### Branches to include in the FEL analysis
Selected 323 branches to include in FEL calculations: `KF790010, CY147300, CY168239, CY171039, KF790389, Node7, Node5, CY141224, CY147305, KF790037, Node13, Node11, KF790403, KF761507, Node18, KC526205, Node17, CY169303, KF789585, CY141202, Node25, Node23, KJ667974, KJ938675, Node30, CY134876, Node29, KF790414, KF790384, KF790408, Node37, Node35, KF886352, KF790438, CY134996, Node43, Node41, KF789591, KF790049, CY134956, CY183153, Node51, Node49, CY168407, CY183065, Node55, KF598733, KC892174, KF685747, CY168471, Node63, Node61, KC892685, KC892641, Node68, KC893110, Node67, KC892480, JX913043, KF551075, CY114509, KC892889, KC893018, Node81, Node79, KC892519, KC892498, Node86, KC892266, Node85, KC892156, JX978746, KC892407, Node93, Node91, KC535402, KC882488, KC535387, Node99, Node97, KC535363, KC535396, KC882883, KC882867, Node107, Node105, KC535378, KC535375, Node111, GQ385891, EU779522, CY037727, FJ179354, Node119, Node117, GQ385889, FJ686933, FJ179356, Node125, Node123, CY173095, CY173191, CY037703, Node132, CY035062, Node131, CY173255, CY044748, GQ385846, Node139, Node137, CY027075, EU199367, CY172823, Node145, Node143, CY172847, CY025643, Node150, CY172839, Node149, CY026251, CY092241, Node156, CY026019, Node155, CY025341, CY172775, CY172903, Node163, Node161, EU199255, CY172431, CY172223, CY172191, CY020069, Node173, Node171, CY092217, CY025485, EU516019, Node179, Node177, CY002080, CY002064, CY002456, CY002048, Node187, Node185, AB434109, CY088198, CY088475, Node194, CY000257, Node193, CY112957, CY006859, Node199, CY000721, CY114493, CY090885, Node205, Node203, CY001792, CY001600, CY002368, Node211, Node209, CY002304, CY006163, CY003632, Node217, Node215, CY001920, CY001912, CY001504, CY006060, Node225, CY001744, CY002136, Node229, CY114309, CY006899, CY112901, Node235, Node233, CY006579, CY006283, Node240, CY007979, Node239, CY006499, CY006491, CY006635, Node247, Node245, CY036847, CY010004, Node252, CY012200, Node251, CY010028, CY009732, Node258, CY010012, Node257, CY010020, CY011416, Node264, CY009484, Node263, CY010036, CY039879, CY039880, Node271, Node269, CY010628, CY010716, CY010516, Node277, Node275, CY012728, CY013701, Node281, CY012760, CY013200, Node286, CY011888, Node285, CY013693, CY012184, CY013669, Node293, Node291, CY112669, CY112556, CY011896, Node299, Node297, CY112605, CY012224, CY012512, CY012896, CY012232, Node309, Node307, CY011848, CY011328, CY114221, Node316, CY011560, Node315, CY012456, CY011824, Node321, CY017283, Node320, Node314, Node312, Node306, Node304, Node302, Node296, Node290, Node284, Node280, Node274, Node268, Node262, Node256, Node250, Node244, Node238, Node232, Node228, Node224, Node222, Node220, Node214, Node208, Node202, Node198, Node192, Node190, Node184, Node182, Node176, Node170, Node168, Node166, Node160, Node154, Node148, Node142, Node136, Node130, Node128, Node122, Node116, Node114, Node110, Node104, Node102, Node96, Node90, Node84, Node78, Node76, Node74, Node72, Node66, Node60, Node58, Node54, Node48, Node46, Node40, Node34, Node28, Node22, Node16, Node10, Node4`


### Obtaining branch lengths and nucleotide rates under the  GTR model
* Log(L) = -7506.06

### Obtaining the global omega estimate based on relative GTR branch lengths and nucleotide substitution biases
* Log(L) = -7302.10
* non-synonymous/synonymous rate ratio for *test* =   0.2923

### Improving branch lengths, nucleotide substitution biases, and global dN/dS ratios under a full codon model
* Log(L) = -7289.65
* non-synonymous/synonymous rate ratio =   0.2598

### For partition 1 these sites are significant at p <=0.1

|     Codon      |   Partition    |     alpha      |      beta      |      LRT       |Selection detected?|
|:--------------:|:--------------:|:--------------:|:--------------:|:--------------:|:-----------------:|
|       20       |       1        |        2.665   |        0.000   |        4.577   |  Neg. p = 0.0324  |
|       32       |       1        |        2.794   |        0.000   |        7.324   |  Neg. p = 0.0068  |
|       33       |       1        |        5.980   |        0.000   |        9.450   |  Neg. p = 0.0021  |
|       39       |       1        |        2.398   |        0.000   |        5.488   |  Neg. p = 0.0192  |
|       43       |       1        |        1.665   |        0.000   |        2.992   |  Neg. p = 0.0837  |
|       48       |       1        |        1.947   |        0.000   |        3.493   |  Neg. p = 0.0616  |
|       51       |       1        |        1.673   |        0.000   |        3.115   |  Neg. p = 0.0776  |
|       52       |       1        |        2.227   |        0.000   |        4.525   |  Neg. p = 0.0334  |
|       56       |       1        |        2.908   |        0.000   |        5.183   |  Neg. p = 0.0228  |
|       64       |       1        |        0.000   |        2.683   |        3.334   |  Pos. p = 0.0679  |
|       67       |       1        |        3.924   |        0.000   |        4.534   |  Neg. p = 0.0332  |
|       68       |       1        |        1.936   |        0.000   |        3.111   |  Neg. p = 0.0778  |
|       72       |       1        |        4.051   |        0.000   |        6.307   |  Neg. p = 0.0120  |
|       77       |       1        |        2.366   |        0.000   |        5.448   |  Neg. p = 0.0196  |
|       79       |       1        |        5.962   |        0.000   |        9.952   |  Neg. p = 0.0016  |
|       80       |       1        |        1.942   |        0.000   |        3.115   |  Neg. p = 0.0776  |
|       85       |       1        |        2.928   |        0.000   |        5.622   |  Neg. p = 0.0177  |
|       89       |       1        |        3.908   |        0.000   |        6.993   |  Neg. p = 0.0082  |
|      101       |       1        |        1.930   |        0.000   |        3.484   |  Neg. p = 0.0620  |
|      103       |       1        |        2.079   |        0.000   |        2.711   |  Neg. p = 0.0997  |
|      106       |       1        |        3.392   |        0.000   |        6.893   |  Neg. p = 0.0087  |
|      107       |       1        |        3.893   |        0.000   |        7.229   |  Neg. p = 0.0072  |
|      113       |       1        |        2.078   |        0.000   |        3.326   |  Neg. p = 0.0682  |
|      130       |       1        |        2.399   |        0.000   |        3.344   |  Neg. p = 0.0675  |
|      131       |       1        |        2.517   |        0.000   |        3.972   |  Neg. p = 0.0463  |
|      132       |       1        |        1.260   |        0.000   |        2.930   |  Neg. p = 0.0870  |
|      133       |       1        |        2.437   |        0.000   |        4.679   |  Neg. p = 0.0305  |
|      142       |       1        |        2.080   |        0.000   |        3.359   |  Neg. p = 0.0668  |
|      146       |       1        |        3.818   |        0.000   |        7.336   |  Neg. p = 0.0068  |
|      152       |       1        |        1.968   |        0.000   |        3.634   |  Neg. p = 0.0566  |
|      154       |       1        |        0.000   |        3.912   |        4.652   |  Pos. p = 0.0310  |
|      159       |       1        |        4.413   |        0.716   |        2.972   |  Neg. p = 0.0847  |
|      164       |       1        |        2.082   |        0.000   |        2.713   |  Neg. p = 0.0995  |
|      176       |       1        |        1.659   |        0.000   |        2.986   |  Neg. p = 0.0840  |
|      177       |       1        |        6.393   |        0.000   |        8.421   |  Neg. p = 0.0037  |
|      181       |       1        |        1.928   |        0.000   |        3.286   |  Neg. p = 0.0699  |
|      190       |       1        |        2.085   |        0.000   |        2.715   |  Neg. p = 0.0994  |
|      201       |       1        |        1.645   |        0.000   |        3.370   |  Neg. p = 0.0664  |
|      208       |       1        |        0.000   |        3.625   |        4.668   |  Pos. p = 0.0307  |
|      216       |       1        |        1.995   |        0.000   |        5.042   |  Neg. p = 0.0247  |
|      225       |       1        |        1.955   |        0.000   |        3.630   |  Neg. p = 0.0567  |
|      229       |       1        |        2.363   |        0.000   |        4.681   |  Neg. p = 0.0305  |
|      233       |       1        |        2.561   |        0.000   |        4.483   |  Neg. p = 0.0342  |
|      234       |       1        |        4.601   |        0.000   |       10.789   |  Neg. p = 0.0010  |
|      238       |       1        |        6.666   |        1.144   |        3.632   |  Neg. p = 0.0567  |
|      244       |       1        |        3.940   |        0.000   |        7.259   |  Neg. p = 0.0071  |
|      252       |       1        |        4.088   |        0.000   |        4.609   |  Neg. p = 0.0318  |
|      255       |       1        |        3.358   |        0.000   |        6.817   |  Neg. p = 0.0090  |
|      261       |       1        |        1.849   |        0.000   |        2.884   |  Neg. p = 0.0895  |
|      266       |       1        |        2.078   |        0.000   |        3.357   |  Neg. p = 0.0669  |
|      281       |       1        |        1.928   |        0.000   |        3.607   |  Neg. p = 0.0575  |
|      285       |       1        |        2.228   |        0.000   |        5.230   |  Neg. p = 0.0222  |
|      296       |       1        |        1.682   |        0.000   |        3.123   |  Neg. p = 0.0772  |
|      301       |       1        |        2.077   |        0.000   |        3.357   |  Neg. p = 0.0669  |
|      305       |       1        |        2.533   |        0.000   |        4.441   |  Neg. p = 0.0351  |
|      310       |       1        |        4.098   |        0.000   |        5.423   |  Neg. p = 0.0199  |
|      315       |       1        |        1.743   |        0.000   |        4.539   |  Neg. p = 0.0331  |
|      317       |       1        |        2.461   |        0.000   |        4.704   |  Neg. p = 0.0301  |
|      318       |       1        |        4.070   |        0.000   |        5.490   |  Neg. p = 0.0191  |
|      321       |       1        |        4.156   |        0.000   |        6.609   |  Neg. p = 0.0101  |
|      329       |       1        |        2.907   |        0.000   |        5.182   |  Neg. p = 0.0228  |
|      331       |       1        |        1.666   |        0.000   |        2.993   |  Neg. p = 0.0836  |
|      348       |       1        |        4.080   |        0.000   |        5.410   |  Neg. p = 0.0200  |
|      349       |       1        |        5.128   |        0.000   |       11.770   |  Neg. p = 0.0006  |
|      351       |       1        |        3.179   |        0.000   |        5.370   |  Neg. p = 0.0205  |
|      352       |       1        |        4.626   |        0.000   |       10.757   |  Neg. p = 0.0010  |
|      356       |       1        |        3.485   |        0.000   |        6.334   |  Neg. p = 0.0118  |
|      358       |       1        |        1.445   |        0.000   |        3.142   |  Neg. p = 0.0763  |
|      364       |       1        |        2.022   |        0.000   |        3.540   |  Neg. p = 0.0599  |
|      371       |       1        |        2.076   |        0.000   |        3.177   |  Neg. p = 0.0747  |
|      373       |       1        |        2.078   |        0.000   |        3.357   |  Neg. p = 0.0669  |
|      375       |       1        |        2.954   |        0.000   |        6.868   |  Neg. p = 0.0088  |
|      376       |       1        |        2.452   |        0.000   |        5.661   |  Neg. p = 0.0173  |
|      378       |       1        |        1.174   |        0.000   |        2.719   |  Neg. p = 0.0992  |
|      380       |       1        |        2.496   |        0.000   |        5.146   |  Neg. p = 0.0233  |
|      383       |       1        |        2.669   |        0.000   |        4.183   |  Neg. p = 0.0408  |
|      386       |       1        |        4.380   |        0.000   |        7.778   |  Neg. p = 0.0053  |
|      404       |       1        |        4.172   |        0.000   |        8.507   |  Neg. p = 0.0035  |
|      405       |       1        |        3.908   |        0.000   |        6.597   |  Neg. p = 0.0102  |
|      412       |       1        |        1.712   |        0.000   |        3.151   |  Neg. p = 0.0759  |
|      413       |       1        |        1.659   |        0.000   |        2.986   |  Neg. p = 0.0840  |
|      414       |       1        |        1.677   |        0.000   |        3.119   |  Neg. p = 0.0774  |
|      415       |       1        |        3.892   |        0.000   |        5.348   |  Neg. p = 0.0207  |
|      417       |       1        |        1.672   |        0.000   |        3.114   |  Neg. p = 0.0776  |
|      418       |       1        |        2.423   |        0.000   |        4.750   |  Neg. p = 0.0293  |
|      419       |       1        |        1.667   |        0.000   |        3.109   |  Neg. p = 0.0779  |
|      423       |       1        |        1.960   |        0.000   |        3.390   |  Neg. p = 0.0656  |
|      424       |       1        |        3.904   |        0.000   |        6.989   |  Neg. p = 0.0082  |
|      432       |       1        |        7.394   |        0.000   |       13.006   |  Neg. p = 0.0003  |
|      438       |       1        |        3.420   |        0.000   |        5.032   |  Neg. p = 0.0249  |
|      440       |       1        |        4.064   |        0.000   |        6.720   |  Neg. p = 0.0095  |
|      441       |       1        |        3.341   |        0.000   |        8.098   |  Neg. p = 0.0044  |
|      446       |       1        |        2.559   |        0.000   |        5.226   |  Neg. p = 0.0223  |
|      449       |       1        |        1.935   |        0.000   |        3.290   |  Neg. p = 0.0697  |
|      451       |       1        |        2.077   |        0.000   |        3.177   |  Neg. p = 0.0747  |
|      454       |       1        |        2.079   |        0.000   |        3.563   |  Neg. p = 0.0591  |
|      464       |       1        |        2.077   |        0.000   |        2.709   |  Neg. p = 0.0998  |
|      477       |       1        |        4.111   |        0.000   |        7.092   |  Neg. p = 0.0077  |
|      481       |       1        |        7.386   |        0.000   |       15.787   |  Neg. p = 0.0001  |
|      482       |       1        |        4.148   |        0.000   |        6.589   |  Neg. p = 0.0103  |
|      492       |       1        |        2.534   |        0.000   |        5.196   |  Neg. p = 0.0226  |
|      493       |       1        |        3.906   |        0.000   |        6.236   |  Neg. p = 0.0125  |
|      498       |       1        |        1.379   |        0.000   |        2.939   |  Neg. p = 0.0864  |
|      504       |       1        |        2.029   |        0.000   |        3.162   |  Neg. p = 0.0754  |
|      508       |       1        |        1.311   |        0.000   |        2.862   |  Neg. p = 0.0907  |
|      509       |       1        |        4.060   |        0.000   |        7.069   |  Neg. p = 0.0078  |
|      511       |       1        |        2.458   |        0.000   |        5.100   |  Neg. p = 0.0239  |
|      512       |       1        |        2.207   |        0.000   |        2.710   |  Neg. p = 0.0997  |
|      517       |       1        |        1.966   |        0.000   |        3.398   |  Neg. p = 0.0653  |
|      519       |       1        |        3.945   |        0.000   |        7.821   |  Neg. p = 0.0052  |
|      520       |       1        |        2.661   |        0.000   |        5.945   |  Neg. p = 0.0148  |
|      522       |       1        |        1.961   |        0.000   |        4.576   |  Neg. p = 0.0324  |
|      523       |       1        |        2.399   |        0.000   |        3.452   |  Neg. p = 0.0632  |
|      526       |       1        |        2.058   |        0.000   |        5.114   |  Neg. p = 0.0237  |
|      540       |       1        |        6.278   |        0.000   |        9.893   |  Neg. p = 0.0017  |
|      541       |       1        |        2.078   |        0.000   |        2.710   |  Neg. p = 0.0997  |
|      548       |       1        |        2.091   |        0.000   |        3.083   |  Neg. p = 0.0791  |
|      557       |       1        |        4.561   |        0.000   |        8.478   |  Neg. p = 0.0036  |

### ** Found _3_ sites under pervasive positive diversifying and _115_ sites under negative selection at p <= 0.1**