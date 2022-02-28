# Anomaly Detection in Time Series: A Comprehensive Evaluation

This is the supporting website for the paper ["Anomaly Detection in Time Series: A Comprehensive Evaluation"][paper].
On this website, we provide the implementations of all algorithms, links to the used datasets, additional algorithm and dataset metadata, as well as further insights from our results that did not make it into the paper.

If you use our artifacts, please consider [citing our paper](#reference).

## Reference

If you use this work or any related software or data artifacts, please cite our paper as follows:

> tbd

Manuscript submitted to [VLDB 2022](https://vldb.org/2022/).

## Motivation

Detecting anomalous subsequences in time series data is an important task in areas ranging from manufacturing processes over finance applications to health care monitoring.
An anomaly can indicate important events, such as production faults, delivery bottlenecks, system defects, or heart flicker, and is therefore of central interest.
The different anomaly types, pattern models, and time series properties led to the development of a multitude of different anomaly detection algorithms, about which various surveys exist [^Blazquez-GarciaEtAl2020review] [^BraeiWagner2020Anomaly] [^ChalapathyChawla2019Deep] [^ChandolaEtAl2012Anomaly] [^ChandolaEtAl2009Anomaly] [^ChoudharyEtAl2017RuntimeEfficacy] [^CookEtAl2020Anomaly] [^GuptaEtAl2014Outlier] [^HodgeAustin2004Survey].
In total, we collected 158 publications about anomaly detection algorithms for time series datasets.
Many of them follow very similar detection approaches, but the general variety of approaches is remarkably high, ranging from simple outlier detection over statistical analysis, signal processing, and data mining to deep learning approaches.
Because all of these approaches exhibit individual strengths and weaknesses, selecting a suitable algorithm for a given anomaly detection task is extremely difficult.

![Univariate time series with scorings of Sub-LOF and LSTM-AD](./figs/univariate-example-ts.png)

The previous Figure, for example, shows that the distance method Sub-LOF detects the point anomaly very well, because it is sensitive to value magnitudes and change amplitudes;
it however fails to detect the subsequence anomaly, because it is insensitive to point orders.
LSTM-AD as a forecasting method, on the contrary, learns normal patterns and heavily relies on seasonality/periodicity;
for this reason, it easily identifies the anomalous subsequence, but since it is robust to noise, it ignores the point anomaly.

Because there is no comprehensive scientific study that evaluates time series anomaly detection algorithms, it is completely unclear how well they perform w. r. t. varying datasets, anomaly types, and parameter settings.
Considering the existing evaluations of individual algorithms, we find that they usually consider only a tiny fraction of related work algorithms and that they are often based on trivial, cherry-picked, biased, mislabeled, unrealistic, or only few datasets.
For this reason, Wu and Keogh even claimed that all "current time series anomaly detection benchmarks are flawed" [^WuKeogh2020Current].
To create a meaningful evaluation, we collected and re-implemented a significant amount of 71 anomaly detection algorithms that represent a broad spectrum of anomaly detection families.
For their evaluation, we put together 967 time series datasets from different domains and generated a bunch of datasets with artificial, but particularly interesting anomalies.
The variety of algorithms and datasets used in this experimental study should provide a clear and reliable picture of the state-of-the-art in time series anomaly detection.

### Overview

In [the paper][paper], we provide practical insights that should help experts to select the optimal algorithm for their anomaly detection task.
Our study also shows the current state-of-the-art in time series anomaly detection and, therefore, serves as an entry point for researchers into the topic.
We indicate potential for future research and, in this way, support the development of new algorithms that are now able to address specific issues, exploit certain capabilities, and ultimately advance the field of anomaly detection.

On this website, we provide the download-links for the datasets and algorithms used in the study.
In addition, we give some further metadata about and insights into data, algorithms, and results:

- [Datasets Overview and Metadata](./notebooks/Datasets.html)
- [Algorithms Overview and Metadata](./notebooks/Algorithms.html)
- Detailed experimental evaluation results ... (tbd)
  - [on our synthetically generated datasets (GutenTAG)](./notebooks/GutenTAG-result-analysis.html)
  - [on all the collected "real-world" datasets](./notebooks/Benchmark-result-analysis.html)
  <!--- (extra) on multivariate, synthetically generated datasets with correlation anomalies -->
- [Case studies](./notebooks/Case-studies.html):
  - [Datasets with no anomalies](./notebooks/Case-studies.html#no-anomalies)
  - [Datasets with a high contamination](./notebooks/Case-studies.html#high-contamination)
  - [Parameter sensitivity](./notebooks/Case-studies.html#parameter-sensitivity)
  - [Detecting anomalies of variable lengths](./notebooks/Detecting-Anomalies-of-Variable-Lengths.html)
  <!--- Large datasets (tbd) -->

### Evaluation Metrics

We use threshold-agnostic evaluation metrics that calculate a single value by comparing the anomaly scorings to the labels. The metrics calculate the area under a curve, which is realized with the Python Package _scikit-learn_ [^sklearn].
The different metrics have different reward and penalize foci.

#### AUC-ROC

The _Area under the Receiver Operator Characteristic Curve_ [^HanleyMcNeil1982AUCROC] [^Bradley1997AUCROC] (AUC-ROC) contrasts the _True Positives Rate_ (TPR) with the _False Positives Rate_ (FPR or Recall). Its focus is on an algorithm's sensitivity.

#### AUC-PR

The _Area under the Precision Recall Curve_ [^Raghavan1989AUCPR] [^Davis2006AUCPR] (AUC-PR) contrasts the _Precision_ with the _Recall_. Its focus is on an algorithm's preciseness.

#### AUC-P<sub>T</sub>R<sub>T</sub>

The _Area under the Range Based Precision Recall Curve_ [^Tatbul2018Range] (AUC-P<sub>T</sub>R<sub>T</sub>) softens the very strict preciseness requirements of AUC-PR to adapt the measure to subsequences. We use the Python Package _prts_ [^prts] to calculate the range-based Precision and Recall values and, further, use them to get the area under its curve. We used the following (default) values for the range-based metrics:

| Parameter | Value |
| --------- | ----- |
|   alpha   |  0.0  |
| cardinality | one |
|    bias   | flat  |

<!--
#### AVERAGE-PRECISION

-->

## Related Resources

- Dataset download-links can be found on the [datasets-page](./notebooks/Datasets.html)
- Source code repositories:
  - Evaluation tool TimeEval: [Github](https://github.com/HPI-Information-Systems/TimeEval)
  - Time series anomaly generator GutenTAG: [Github](https://github.com/HPI-Information-Systems/gutentag)
  - Algorithm source code (and necessary docker images): [Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms)
- [HPI umbrella project](https://hpi.de/naumann/projects/distributed-computing/efficient-subsequence-anomaly-detection-on-time-series-data.html)

## References

[^WuKeogh2020Current]: Wu, Renjie, and Eamonn J. Keogh. "Current Time Series Anomaly Detection Benchmarks Are Flawed and Are Creating the Illusion of Progress." ArXiv:2009.13807 [Cs, Stat], 2020. http://arxiv.org/abs/2009.13807.
[^Blazquez-GarciaEtAl2020review]: Blázquez-García, Ane, Angel Conde, Usue Mori, and Jose A. Lozano. "A Review on Outlier/Anomaly Detection in Time Series Data." ArXiv:2002.04236 [Cs, Stat], 2020. http://arxiv.org/abs/2002.04236.
[^BraeiWagner2020Anomaly]: Braei, Mohammad, and Sebastian Wagner. "Anomaly Detection in Univariate Time-Series: A Survey on the State-of-the-Art." ArXiv:2004.00433 [Cs, Stat], 2020. http://arxiv.org/abs/2004.00433.
[^ChalapathyChawla2019Deep]: Chalapathy, Raghavendra, and Sanjay Chawla. "Deep Learning for Anomaly Detection: A Survey." ArXiv:1901.03407 [Cs, Stat], 2019. http://arxiv.org/abs/1901.03407.
[^ChandolaEtAl2012Anomaly]: Chandola, V., A. Banerjee, and V. Kumar. "Anomaly Detection for Discrete Sequences: A Survey." IEEE Transactions on Knowledge and Data Engineering (TKDE) 24, no. 5 (2012): 823–39. https://doi.org/10.1109/TKDE.2010.235.
[^ChandolaEtAl2009Anomaly]: Chandola, Varun, Arindam Banerjee, and Vipin Kumar. "Anomaly Detection: A Survey." ACM Computing Surveys 41, no. 3 (2009): 1–58. https://doi.org/10.1145/1541880.1541882.
[^ChoudharyEtAl2017RuntimeEfficacy]: Choudhary, Dhruv, Arun Kejariwal, and Francois Orsini. "On the Runtime-Efficacy Trade-off of Anomaly Detection Techniques for Real-Time Streaming Data." ArXiv:1710.04735 [Cs, Eess, Stat], 2017. http://arxiv.org/abs/1710.04735.
[^CookEtAl2020Anomaly]: Cook, Andrew A., Goksel Misirli, and Zhong Fan. "Anomaly Detection for IoT Time-Series Data: A Survey." IEEE Internet of Things Journal 7, no. 7 (2020): 6481–94. https://doi.org/10.1109/JIOT.2019.2958185.
[^GuptaEtAl2014Outlier]: Gupta, Manish, Jing Gao, Charu C. Aggarwal, and Jiawei Han. "Outlier Detection for Temporal Data: A Survey." IEEE Transactions on Knowledge and Data Engineering (TKDE) 26, no. 9 (2014): 2250–67. https://doi.org/10.1109/TKDE.2013.184.
[^HodgeAustin2004Survey]: Hodge, Victoria J., and Jim Austin. "A Survey of Outlier Detection Methodologies." Artificial Intelligence Review 22, no. 2 (2004): 85–126. https://doi.org/10.1007/s10462-004-4304-y.
[^sklearn]: Pedregosa, F., G. Varoquaux, A. Gramfort, V. Michel, B. Thirion, O. Grisel, M. Blondel, et al. “Scikit-Learn: Machine Learning in Python.” Journal of Machine Learning Research 12 (2011): 2825–2830.
[^HanleyMcNeil1982AUCROC]: Hanley, James A, and Barbara J McNeil. “The Meaning and Use of the Area under a Receiver Operating Characteristic (ROC) Curve.” Radiology 143, no. 1 (1982): 29–36.
[^Bradley1997AUCROC]: Bradley, Andrew P. “The Use of the Area under the ROC Curve in the Evaluation of Machine Learning Algorithms.” Pattern Recognition 30, no. 7 (1997): 1145–1159.
[^Raghavan1989AUCPR]: Raghavan, Vijay, Peter Bollmann, and Gwang S Jung. “A Critical Investigation of Recall and Precision as Measures of Retrieval System Performance.” ACM Transactions on Information Systems (TOIS) 7, no. 3 (1989): 205–229.
[^Davis2006AUCPR]: Davis, Jesse, and Mark Goadrich. “The Relationship between Precision-Recall and ROC Curves.” In Proceedings of the 23rd International Conference on Machine Learning, 233–240, 2006.
[^prts]: https://pypi.org/project/prts/
[^Tatbul2018Range]: Tatbul, Nesime, Tae Jun Lee, Stan Zdonik, Mejbah Alam, and Justin Gottschlich. “Precision and Recall for Time Series.” ArXiv Preprint ArXiv:1803.03639, 2018.


[paper]: # "paper download link pending"
