# Machine_Learning_Supervised_Algorithms
Datasets:
https://drive.google.com/open?id=0BxnjqxEVUcSTYk5nbEZQcXNWT0k

Decision Trees:
weka.classifiers.trees.J48 -C 0.25 -M 2

Adaboost:
weka.classifiers.meta.AdaBoostM1 -P 100 -S 1 -I 10 -W weka.classifiers.trees.DecisionStump

Artificial Neural Networks:
weka.classifiers.functions.MultilayerPerceptron -L 0.3 -M 0.2 -N 500 -V 0 -S 0 -E 20 -H a

Support Vector Machines:
weka.classifiers.functions.SMO -C 1.0 -L 0.001 -P 1.0E-12 -N 0 -V -1 -W 1 -K "weka.classifiers.functions.supportVector.PolyKernel -E 1.0 -C 250007" -calibrator "weka.classifiers.functions.Logistic -R 1.0E-8 -M -1 -num-decimal-places 4"

K Nearest Neighbors:
weka.classifiers.lazy.IBk -K 1 -W 0 -A "weka.core.neighboursearch.LinearNNSearch -A \"weka.core.EuclideanDistance -R first-last\""

Used Experimenter to configure different runs for all the algorithms with increasing data size for both testing on test and cross validation data.
Manually ran algorithms on each training data size to test on train data.
