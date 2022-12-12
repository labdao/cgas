#cgas 

## about
an [[abcellera]] company - based on work by [[gianni de fabritiis]] that is focused on [[machine learning]] tools for in-silico [[small molecule]] drug discovery

## overview
![[Pasted image 20221212095747.png]]

## [[target identification]] 
### [[receptor preparation]]
 - [[pm proteinprepare]]
 - ace profiler - [[homology]] search across [[PDB]] based on sequence

### [[molecular dynamics]]
* 1. [[pm system builder]]
* 2. [[pm simple run]] - [[@doerrHTMDHighThroughputMolecular2016]]
* 3. [[pm isca]] - [[adaptive sampling molecular dynamics]] - [[@doerrOntheFlyLearningSampling2014]]

other: [[membrane]] builder

### [[binding site]] 
[[pm cryptic scout]] - check for crytpic [[binding site]]
[[pm plexview]] - vis interaction given ligand and protein
[[deepsite]] - [[binding site]] identification

## [[small molecule]]
### [[ligand preparation]]
[[pm aceprep]] - [[ligand preparation]] and [[conformer]] generation

### representation search 
pathwaymap based on [[ECFP4]] fingerprint

### ligand generation 
generative - [[crem]] 

## [[docking]]
[[pm isba]] - [[adaptive sampling molecular dynamics]] [[@doerrOntheFlyLearningSampling2014]]
[[kdeep]] - [[@jimenezKDEEPProteinLigand2018]]
[[acedock]] - based on [[rdock]] - requires a [[template ligand]]


## questions
* interesting models
	* [[crem]] implementation - is the user supplying their fragment library to you?
	* parameterize - 
	* [[adaptive sampling molecular dynamics]]
		* seems like difference between isba and isca is focus on protein-ligand vs. protein -protein interaction
		* isba - can we use it to score docked poses for stability?
* is there an API for models?
* how do you version the containers? does the user receive the version?

## related links
[[@doerrTorchMDDeepLearning2021]] - [[stefan doerr]]
