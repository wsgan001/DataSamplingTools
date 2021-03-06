******************************************************************************
			Author: Barnan Das
			Email: barnandas@wsu.edu
			Homepage: www.eecs.wsu.edu/~bdas1
			Last Updated: June 25, 2012
******************************************************************************

File Descriptions:
weka.jar -> Weka jar file that is called by several Matlab scripts in this 
	    directory.

train.arff, test.arff -> ARFF (Weka compatible) files generated by some of the 
			 Matlab scripts.

ARFFheader.txt -> Defines the ARFF header for the data file "data.csv". Please
		  refer to the following link to learn more about ARFF format.
		  http://www.cs.waikato.ac.nz/ml/weka/arff.html

Att_values.m -> Contains the attribute values for the dataset. * Varies as per 
		dataset.

TAN.m -> Contains the conditional probability matrix built by the Bayesian 
	 tree which is generated by Weka machine learning software using TAN.
	 Tan or Tree Augmented Naive Bayes is a search algorithm for the
	 BayesNet classifier of Weka.

GibbsSampler.m -> Implementation of Gibbs sampler that uses attribute 
		  dependencies imposed by the Bayesian tree and stored in 
		  TAN.m.

WrapperGibbsSampler.m -> Implementation of the wrapper-based Gibbs sampler. 
			 The attribute dependencies imposed by the Bayesian 
			 tree and stored in TAN.m.

RACOG.m -> The RACOG algorithm that runs for 5 folds and evaluates its 
	   performance by testing the oversampled dataset with four 
	   classifiers.

wRACOG.m -> The wRACOG algorithm that runs for 5 folds and evaluates its 
	    performance by testing the oversampled dataset with four 
	    classifiers.

ClassifierTrain.m, ClassifierPredict.m, CSVtoARFF.m -> Matlab functions used by 
						       RACOG.m and wRACOG.m


**************************************xxx**************************************