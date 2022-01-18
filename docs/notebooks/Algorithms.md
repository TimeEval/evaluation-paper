---
title: Algorithms
description: This page lists all algorithms with implementation and parametrization information used in the experimental evaluation paper.

---

<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript" async></script>
<script>
  var require = {
    enforceDefine: true,
    waitSeconds: 30, // only give up loading a module after 30s (default: 7s)
  };
</script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js" type="text/javascript"></script>

# Algorithms Overview and Metadata

We collected __158__ time series anomaly detection algorithms from different research areas; _Deep Learning_, _Statistics_, _Outlier Detection_, _Signal Analysis_, _Classic Machine Learning_, _Data Mining_, _Stochastic Learning_. Some of these algorithms can detect anomalies on multidimensional time series.

## Overview

We implemented __71__ of the total collection. These implemented algorithms are used in our evaluation. The following table shows all categorized algorithms. Column _Implemented_ shows which algorithms we used in the evaluation.

<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Research Area</th>
      <th>Method data type</th>
      <th>Implemented</th>
    </tr>
    <tr>
      <th>Method Name</th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>AE</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>ARIMA</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Bagel</th>
      <td>Deep Learning</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>CBLOF</th>
      <td>Ourlier Detection</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>COF</th>
      <td>Ourlier Detection</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>COPOD</th>
      <td>Ourlier Detection</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>DAE</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>DBStream</th>
      <td>Ourlier Detection</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>DSPOT</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>DWT-MLEAD</th>
      <td>Signal Analysis</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>DeepAnT</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>DeepNAP</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Donut</th>
      <td>Deep Learning</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>EIF</th>
      <td>Classic Machine Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>EncDec-AD</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Ensemble GI</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>FFT</th>
      <td>Signal Analysis</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Fast-MCD</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>GrammarViz</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>HBOS</th>
      <td>Classic Machine Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>HIF</th>
      <td>Ourlier Detection</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>HOT SAX</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>HealthESN</th>
      <td>Deep Learning</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Hybrid KNN</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>IE-CAE</th>
      <td>Deep Learning</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>IF-LOF</th>
      <td>Ourlier Detection</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>KNN</th>
      <td>Classic Machine Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>LOF</th>
      <td>Ourlier Detection</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>LSTM-AD</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>LSTM-VAE</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>LaserDBN</th>
      <td>Stochastic Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Left STAMPi</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>MSCRED</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>MTAD-GAT</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>MedianMethod</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>MultiHMM</th>
      <td>Stochastic Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>NormA</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Normalizing Flows</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>NoveltySVR</th>
      <td>Classic Machine Learning</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>NumentaHTM</th>
      <td>Deep Learning</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>OceanWNN</th>
      <td>Deep Learning</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>OmniAnomaly</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>PCC</th>
      <td>Classic Machine Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>PCI</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>PS-SVM</th>
      <td>Classic Machine Learning</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>PST</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>RBForest</th>
      <td>Classic Machine Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>RForest</th>
      <td>Classic Machine Learning</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>RobustPCA</th>
      <td>Classic Machine Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>S-H-ESD</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>SAND</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>SARIMA</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>SR</th>
      <td>Signal Analysis</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>SR-CNN</th>
      <td>Deep Learning</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>SSA</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>STAMP</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>STOMP</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Series2Graph</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Sub-Fast-MCD</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Sub-IF</th>
      <td>Ourlier Detection</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Sub-LOF</th>
      <td>Ourlier Detection</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>TARZAN</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>TAnoGAN</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>TSBitmap</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Telemanom</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Torsk</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>Triple ES</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>VALMOD</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>XGBoosting</th>
      <td>Classic Machine Learning</td>
      <td>univariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>iForest</th>
      <td>Ourlier Detection</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>k-Means</th>
      <td>Classic Machine Learning</td>
      <td>multivariate</td>
      <td>True</td>
    </tr>
    <tr>
      <th>AD-LTI</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>AMD Segmentation</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>ANODE</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>AOSVM</th>
      <td>Classic Machine Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>AR</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>ARMA</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>BLOF</th>
      <td>Ourlier Detection</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>BoehmerGraph</th>
      <td>Data Mining</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>Box Plot</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>CHEB</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>CoalESN</th>
      <td>Deep Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>ConInd</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>CxDBN</th>
      <td>Stochastic Learning</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>DAD</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>DADS</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>DILOF</th>
      <td>Ourlier Detection</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>Deep K-Means</th>
      <td>Deep Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>Deep OCSVM</th>
      <td>Deep Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>DeepLSTM</th>
      <td>Deep Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>DeepPCA</th>
      <td>Deep Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>DissimilarityAlgo</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>Double ES (Holt's)</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>Dynamic State Estimator (DSE)</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>EDBN</th>
      <td>Stochastic Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>EM-HMM</th>
      <td>Stochastic Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>EWMA-STR</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>Eros-SVMs</th>
      <td>Classic Machine Learning</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>FuzzyDNBC</th>
      <td>Stochastic Learning</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>GLA</th>
      <td>Stochastic Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>GeckoFSM</th>
      <td>Ourlier Detection</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>GridLOF</th>
      <td>Ourlier Detection</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>HMAD</th>
      <td>Stochastic Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>HSDE</th>
      <td>Ourlier Detection</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>HSMM</th>
      <td>Stochastic Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>Hybrid K-means</th>
      <td>Classic Machine Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>I-HMM</th>
      <td>Stochastic Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>ILOF</th>
      <td>Data Mining</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>K-LOF</th>
      <td>Ourlier Detection</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>KNN (PTSA)</th>
      <td>Classic Machine Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>Kalman Filter</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>KnorrSeq2</th>
      <td>Data Mining</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>LAMP (GPU)</th>
      <td>Deep Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>LOCI/aLOCI</th>
      <td>Ourlier Detection</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>LSTM (PTSA)</th>
      <td>Deep Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>LSTM-based VAE-GAN</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>MA</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>MAD-GAN</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>MCD</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>MCOD</th>
      <td>Ourlier Detection</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>MERLIN</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>MGDD</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>MS-SVDD</th>
      <td>Classic Machine Learning</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>MoteESN</th>
      <td>Deep Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>MultiHTM</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>NetworkSVM</th>
      <td>Classic Machine Learning</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>NorM</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>NorM (SAD)</th>
      <td>Data Mining</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>OC-KFD</th>
      <td>Classic Machine Learning</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>Online DWT-MLEAD</th>
      <td>Signal Analysis</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>PAD</th>
      <td>Deep Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>PCA</th>
      <td>Classic Machine Learning</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>Poly (PTSA)</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>RADM</th>
      <td>Deep Learning</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>RPIF</th>
      <td></td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>RUSBoost</th>
      <td>Classic Machine Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>RePAD</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>Robust Deep AutoEncoder</th>
      <td>Deep Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>S-SVM</th>
      <td>Classic Machine Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>SALOF</th>
      <td>Ourlier Detection</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>SCRIMP++</th>
      <td>Data Mining</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>SH-ESD+</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>SLADE-MTS</th>
      <td>Classic Machine Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>SLADE-TS</th>
      <td>Classic Machine Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>STORN</th>
      <td>Deep Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>Simple ES (EWMA)</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>SmartSifter</th>
      <td>Stochastic Learning</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>Sparse AutoEncoder</th>
      <td>Deep Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>Structured Denoising AutoEncoder (StrDAE)</th>
      <td>Deep Learning</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>SurpriseEncoding</th>
      <td>Data Mining</td>
      <td>multivariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>TCN-AE</th>
      <td>Deep Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>TOLF</th>
      <td>Ourlier Detection</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>TwoFinger</th>
      <td>Data Mining</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>U-GMM-HMM</th>
      <td>Stochastic Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>VELC</th>
      <td>Deep Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>Yesterday (PTSA)</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
    <tr>
      <th>pEWMA</th>
      <td>Statistics (Regression &amp; Forecasting)</td>
      <td></td>
      <td>False</td>
    </tr>
    <tr>
      <th>sequenceMiner</th>
      <td>Classic Machine Learning</td>
      <td>univariate</td>
      <td>False</td>
    </tr>
  </tbody>
</table>
</div>

## Implementation Details

More than half of the __71__ chosen algorithms had to be reimplemented by ourselves. However, some authors provided algorithm implementations or community versions exist. All implementations can be found in [our Github repository](https://github.com/HPI-Information-Systems/TimeEval-algorithms).

|Method Name|Source Code Origin|Language|License|Method Family||
|---|---|---|---|---|---|
|ARIMA|own (John Paparrizos and team)|Python|no license|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/arima)|
|AE|own|Python, Tensorflow|MIT|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/autoencoder)|
|Bagel|original|Python|no license|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/bagel)|
|CBLOF|community (PyOD)|Python|BSD 2|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/cblof)|
|COF|community (PyOD)|Python|BSD 2|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/cof)|
|COPOD|community (PyOD)|Python|BSD 2|distribution|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/copod)|
|DAE|own|Python, Tensorflow|MIT|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/dae)|
|DBStream|original|R|no license|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/dbstream)|
|DeepAnT|own|Python, Pytorch|no license|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/deepant)|
|DeepNAP|own|Python, Pytorch|MIT|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/deepnap)|
|Donut|original|Python, Pytorch|no license|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/donut)|
|DSPOT|original|Python|GPL 3.0|distribution|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/dspot)|
|DWT-MLEAD|own|Python|MIT|distribution|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/dwt_mlead)|
|EIF|original|Python|UIUC|trees|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/eif)|
|EncDec-AD|own|Python, Pytorch|MIT|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/encdec_ad)|
|Ensemble GI|own|Python|MIT|encoding|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/ensemble_gi)|
|Fast-MCD|own|Python|MIT|distribution|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/fast_mcd)|
|FFT|own|Python|MIT|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/fft)|
|RForest|own|Python|MIT|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/generic_rf)|
|XGBoosting|own|Python|MIT|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/generic_xgb)|
|GrammarViz|original|Java|GPL 2.0|encoding|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/grammarviz3)|
|HBOS|community (PyOD)|Python|BSD 2|distribution|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/hbos)|
|HealthESN|own|Python|MIT|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/health_esn)|
|HIF|original|Python|GPL 2.0|trees|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/hif)|
|HOT SAX|original|Python|GPL 2.0|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/hotsax)|
|Hybrid KNN|own|Python, Pytorch|MIT|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/hybrid_knn)|
|IF-LOF|own|Python|MIT|trees|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/if_lof)|
|iForest|community (PyOD)|Python|BSD 2|trees|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/iforest)|
|IE-CAE|own|Python, Pytorch|MIT|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/img_embedding_cae)|
|k-Means|own|Python|MIT|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/kmeans)|
|KNN|community (PyOD)|Python|BSD 2|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/knn)|
|LaserDBN|own|Python|MIT|encoding|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/laser_dbn)|
|Left STAMPi|original|Python|BSD|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/left_stampi)|
|LOF|community (PyOD)|Python|BSD 2|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/lof)|
|LSTM-AD|own|Python, Pytorch|MIT|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/lstm_ad)|
|LSTM-VAE|own|Python, Tensorflow|MIT|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/lstm_vae)|
|MedianMethod|own|Python|MIT|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/median_method)|
|MSCRED|own|Python, Tensorflow|MIT|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/mscred)|
|MTAD-GAT|own|Python, Pytorch|MIT|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/mtad_gat)|
|MultiHMM|own|Python|MIT|encoding|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/multi_hmm)|
|NormA|original|Python|private|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/norma)|
|Normalizing Flows|own|Python, Pytorch|MIT|distribution|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/normalizing_flows)|
|NoveltySVR|own|Python|GPL 3.0|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/novelty_svr)|
|NumentaHTM|original|Python|AGPL|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/numenta_htm)|
|OceanWNN|own|Python, Pytorch|MIT|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/ocean_wnn)|
|OmniAnomaly|original|Python, Tensorflow|MIT|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/omnianomaly)|
|PCC|community (PyOD)|Python|BSD 2|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/pcc)|
|PCI|own|Python|MIT|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/pci)|
|PS-SVM|own|Python|MIT|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/phasespace_svm)|
|PST|own|R|GPL|encoding|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/pst)|
|RBForest|own|Python|MIT|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/random_black_forest)|
|RobustPCA|community|Python|MIT|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/robust_pca)|
|S-H-ESD|own|R|GPL 3.0|distribution|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/s_h_esd)|
|SAND|original|Python|private|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/sand)|
|SARIMA|own|Python|BSD 3.0|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/sarima)|
|Series2Graph|original|Python|private|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/series2graph)|
|SR|original|Python|MIT|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/sr)|
|SR-CNN|original|Python, Pytorch|MIT|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/sr_cnn)|
|SSA|own (John Paparrizos and team)|Python|no license|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/ssa)|
|STAMP|original|R|Apache|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/stamp)|
|STOMP|original|R|Apache|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/stomp)|
|Sub-Fast-MCD|own|Python|MIT|distribution|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/subsequence_fast_mcd)|
|Sub-IF|own|Python|MIT|trees|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/subsequence_if)|
|Sub-LOF|own|Python|MIT|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/subsequence_lof)|
|TAnoGAN|own|Python, Pytorch|no license|reconstruction|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/tanogan)|
|TARZAN|original|Python|no license|encoding|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/tarzan)|
|Telemanom|original|Python, Tensorflow|Caltech|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/telemanom)|
|Torsk|original|Python, Pytorch|no license|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/torsk)|
|Triple ES|own|Python|MIT|forecasting|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/triple_es)|
|TSBitmap|community|Python|no license|encoding|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/ts_bitmap)|
|VALMOD|original|R|Apache|distance|[→Github](https://github.com/HPI-Information-Systems/TimeEval-algorithms/blob/main/valmod)|

## Parameterization

After an independent parameter search, we conducted the experiments with the following parameters. Some parameters depend on data set properties.

### ARIMA

|Parameter|Value|
|---|---|
|window_size|1.0 dataset period size|
|max_lag|10% of dataset length|
|p_start|1|
|q_start|1|
|max_p|5|
|max_q|5|
|differencing_degree|1|
|distance_metric|twed|
|random_state|42|

### AE

|Parameter|Value|
|---|---|
|latent_size|32|
|epochs|500|
|learning_rate|0.001|
|split|0.8|
|early_stopping_delta|0.05|
|early_stopping_patience|10|
|random_state|42|

### Bagel

|Parameter|Value|
|---|---|
|window_size|2.0 dataset period size|
|latent_size|6|
|hidden_layer_shape|[100, 100]|
|dropout|0.1|
|cuda|False|
|epochs|500|
|batch_size|64|
|split|0.8|
|early_stopping_delta|0.05|
|early_stopping_patience|10|
|random_state|42|

### CBLOF

|Parameter|Value|
|---|---|
|n_clusters|50|
|alpha|default|
|beta|default|
|use_weights|default|
|random_state|42|
|n_jobs|1|

### COF

|Parameter|Value|
|---|---|
|n_neighbors|50|
|random_state|42|

### COPOD

|Parameter|Value|
|---|---|
|random_state|42|

### DAE

|Parameter|Value|
|---|---|
|latent_size|32|
|epochs|500|
|learning_rate|0.001|
|noise_ratio|0.1|
|split|0.8|
|early_stopping_delta|0.05|
|early_stopping_patience|10|
|random_state|42|

### DBStream

|Parameter|Value|
|---|---|
|window_size|1.0 dataset period size|
|radius|1.3|
|lambda|0.001|
|distance_metric|euclidean|
|shared_density|True|
|n_clusters|30|
|alpha|0.5|
|min_weight|0|
|random_state|42|

### DeepAnT

|Parameter|Value|
|---|---|
|epochs|500|
|window_size|0.5 dataset period size|
|prediction_window_size|50|
|learning_rate|0.001|
|batch_size|64|
|random_state|42|
|split|0.8|
|early_stopping_delta|0.05|
|early_stopping_patience|10|

### DeepNAP

|Parameter|Value|
|---|---|
|anomaly_window_size|max anomaly length|
|partial_sequence_length|3|
|lstm_layers|1|
|rnn_hidden_size|200|
|dropout|0.5|
|linear_hidden_size|100|
|batch_size|64|
|validation_batch_size|64|
|epochs|500|
|learning_rate|0.001|
|split|0.8|
|early_stopping_delta|0.05|
|early_stopping_patience|10|
|random_state|42|

### Donut

|Parameter|Value|
|---|---|
|window_size|1.0 dataset period size|
|latent_size|5|
|regularization|0.001|
|linear_hidden_size|130|
|epochs|500|
|random_state|42|

### DSPOT

|Parameter|Value|
|---|---|
|q|default|
|n_init|1000|
|level|0.99|
|up|True|
|down|True|
|alert|default|
|bounded|True|
|max_excess|200|
|random_state|42|

### DWT-MLEAD

|Parameter|Value|
|---|---|
|start_level|3|
|quantile_epsilon|0.1|
|random_state|42|

### EIF

|Parameter|Value|
|---|---|
|n_trees|500|
|max_samples|None|
|extension_level|None|
|limit|None|
|random_state|42|

### EncDec-AD

|Parameter|Value|
|---|---|
|lstm_layers|3|
|anomaly_window_size|max anomaly length|
|latent_size|-30% default value|
|batch_size|64|
|validation_batch_size|64|
|epochs|500|
|split|0.8|
|early_stopping_delta|0.05|
|early_stopping_patience|10|
|learning_rate|0.001|
|random_state|42|
|window_size|1.0 dataset period size|
|test_batch_size|64|

### Ensemble GI

|Parameter|Value|
|---|---|
|anomaly_window_size|max anomaly length|
|n_estimators|500|
|max_paa_transform_size|20|
|max_alphabet_size|10|
|selectivity|0.8|
|random_state|42|
|n_jobs|1|
|window_method|sliding|

### Fast-MCD

|Parameter|Value|
|---|---|
|store_precision|True|
|support_fraction|default|
|random_state|42|

### FFT

|Parameter|Value|
|---|---|
|fft_parameters|3|
|context_window_size|5|
|local_outlier_threshold|0.78|
|max_anomaly_window_size|max anomaly length|
|max_sign_change_distance|20|
|random_state|42|

### RForest

|Parameter|Value|
|---|---|
|train_window_size|500|
|n_trees|500|
|max_features_method|auto|
|bootstrap|True|
|max_samples|None|
|random_state|42|
|verbose|0|
|n_jobs|1|
|max_depth|4|
|min_samples_split|2|
|min_samples_leaf|1|

### XGBoosting

|Parameter|Value|
|---|---|
|train_window_size|500|
|n_estimators|500|
|learning_rate|0.001|
|booster|gbtree|
|tree_method|auto|
|n_trees|500|
|max_depth|4|
|max_samples|None|
|colsample_bytree|None|
|colsample_bylevel|None|
|colsample_bynode|None|
|random_state|42|
|verbose|0|
|n_jobs|1|

### GrammarViz

|Parameter|Value|
|---|---|
|anomaly_window_size|max anomaly length|
|paa_transform_size|5|
|alphabet_size|6|
|normalization_threshold|0.01|
|random_state|42|

### HBOS

|Parameter|Value|
|---|---|
|n_bins|20|
|alpha|default|
|bin_tol|default|
|random_state|42|

### HealthESN

|Parameter|Value|
|---|---|
|linear_hidden_size|default|
|prediction_window_size|50|
|connectivity|default|
|spectral_radius|default|
|activation|default|
|random_state|42|

### HIF

|Parameter|Value|
|---|---|
|n_trees|500|
|max_samples|None|
|random_state|42|

### HOT SAX

|Parameter|Value|
|---|---|
|num_discords|None|
|anomaly_window_size|max anomaly length|
|paa_transform_size|3|
|alphabet_size|3|
|normalization_threshold|0.01|
|random_state|42|

### Hybrid KNN

|Parameter|Value|
|---|---|
|linear_layer_shape|default|
|split|0.8|
|anomaly_window_size|max anomaly length|
|batch_size|64|
|test_batch_size|64|
|epochs|500|
|early_stopping_delta|0.05|
|early_stopping_patience|10|
|learning_rate|0.001|
|n_neighbors|10|
|n_estimators|500|
|random_state|42|

### IF-LOF

|Parameter|Value|
|---|---|
|n_trees|500|
|max_samples|default|
|n_neighbors|50|
|alpha|default|
|m|default|
|random_state|42|

### iForest

|Parameter|Value|
|---|---|
|n_trees|500|
|max_samples|None|
|max_features|1.0|
|bootstrap|false|
|random_state|42|
|verbose|0|
|n_jobs|1|

### IE-CAE

|Parameter|Value|
|---|---|
|anomaly_window_size|max anomaly length|
|kernel_size|default|
|num_kernels|32|
|latent_size|100|
|leaky_relu_alpha|0.03|
|batch_size|64|
|test_batch_size|64|
|learning_rate|0.001|
|epochs|500|
|split|0.8|
|early_stopping_delta|0.05|
|early_stopping_patience|10|
|random_state|42|

### k-Means

|Parameter|Value|
|---|---|
|n_clusters|50|
|anomaly_window_size|max anomaly length|
|stride|1|
|n_jobs|1|
|random_state|42|

### KNN

|Parameter|Value|
|---|---|
|n_neighbors|50|
|leaf_size|20|
|method|default|
|radius|default|
|distance_metric_order|2|
|n_jobs|1|
|random_state|42|

### LaserDBN

|Parameter|Value|
|---|---|
|timesteps|2|
|n_bins|10|
|random_state|42|

### Left STAMPi

|Parameter|Value|
|---|---|
|anomaly_window_size|max anomaly length|
|n_init_train|10% of dataset length or until first anomaly|
|random_state|42|

### LOF

|Parameter|Value|
|---|---|
|n_neighbors|50|
|leaf_size|20|
|distance_metric_order|2|
|n_jobs|1|
|random_state|42|

### LSTM-AD

|Parameter|Value|
|---|---|
|lstm_layers|1|
|split|0.8|
|window_size|2.0 dataset period size|
|prediction_window_size|50|
|batch_size|64|
|validation_batch_size|64|
|epochs|500|
|early_stopping_delta|0.05|
|early_stopping_patience|10|
|learning_rate|0.001|
|random_state|42|
|test_batch_size|64|

### LSTM-VAE

|Parameter|Value|
|---|---|
|rnn_hidden_size|5|
|latent_size|5|
|learning_rate|0.001|
|batch_size|64|
|epochs|500|
|window_size|1.0 dataset period size|
|lstm_layers|10|
|early_stopping_delta|0.05|
|early_stopping_patience|10|

### MedianMethod

|Parameter|Value|
|---|---|
|neighbourhood_size|2.0 dataset period size|
|random_state|42|

### MSCRED

|Parameter|Value|
|---|---|
|windows|default|
|gap_time|10|
|window_size|1.0 dataset period size|
|batch_size|64|
|learning_rate|0.001|
|epochs|500|
|early_stopping_patience|10|
|early_stopping_delta|0.05|
|split|0.8|
|test_batch_size|64|
|random_state|42|

### MTAD-GAT

|Parameter|Value|
|---|---|
|mag_window_size|40|
|score_window_size|52|
|threshold|6|
|context_window_size|30|
|kernel_size|7|
|learning_rate|0.001|
|epochs|500|
|batch_size|64|
|window_size|2.0 dataset period size|
|gamma|0.8|
|latent_size|5|
|linear_layer_shape|[5, 5, 5]|
|early_stopping_patience|10|
|early_stopping_delta|0.05|
|split|0.8|
|random_state|42|

### MultiHMM

|Parameter|Value|
|---|---|
|discretizer|choquet|
|n_bins|5|
|random_state|42|

### NormA

|Parameter|Value|
|---|---|
|anomaly_window_size|max anomaly length|
|normal_model_percentage|0.5|
|random_state|42|

### Normalizing Flows

|Parameter|Value|
|---|---|
|n_hidden_features_factor|1.0|
|hidden_layer_shape|[100, 100]|
|window_size|1.0 dataset period size|
|split|0.8|
|epochs|500|
|batch_size|64|
|test_batch_size|64|
|teacher_epochs|100|
|distillation_iterations|100|
|percentile|0.05|
|early_stopping_patience|10|
|early_stopping_delta|0.05|
|random_state|42|

### NoveltySVR

|Parameter|Value|
|---|---|
|n_init_train|10% of dataset length or until first anomaly|
|forgetting_time|None|
|train_window_size|500|
|anomaly_window_size|max anomaly length|
|lower_suprise_bound|None|
|scaling|standard|
|epsilon|0.1|
|verbose|0|
|C|1.0|
|kernel|rbf|
|degree|3|
|gamma|None|
|coef0|0.0|
|tol|0.001|
|stabilized|True|
|random_state|42|

### NumentaHTM

|Parameter|Value|
|---|---|
|encoding_input_width|21|
|encoding_output_width|75|
|autoDetectWaitRecords|50|
|columnCount|2048|
|numActiveColumnsPerInhArea|50|
|potentialPct|0.1|
|synPermConnected|0.1|
|synPermActiveInc|0.05|
|synPermInactiveDec|0.01|
|cellsPerColumn|32|
|inputWidth|2048|
|newSynapseCount|15|
|maxSynapsesPerSegment|32|
|maxSegmentsPerCell|128|
|initialPerm|0.15|
|permanenceInc|0.1|
|permanenceDec|0.1|
|globalDecay|0|
|maxAge|0|
|minThreshold|9|
|activationThreshold|12|
|pamLength|1|
|alpha|0.5|
|random_state|42|

### OceanWNN

|Parameter|Value|
|---|---|
|train_window_size|500|
|hidden_size|20|
|batch_size|64|
|test_batch_size|64|
|epochs|500|
|split|0.8|
|early_stopping_delta|0.05|
|early_stopping_patience|10|
|learning_rate|0.001|
|wavelet_a|-3.25|
|wavelet_k|-1.95|
|wavelet_wbf|mexican_hat|
|wavelet_cs_C|2.275|
|threshold_percentile|0.99|
|random_state|42|
|with_threshold|True|

### OmniAnomaly

|Parameter|Value|
|---|---|
|latent_size|4|
|rnn_hidden_size|100|
|window_size|1.0 dataset period size|
|linear_hidden_size|100|
|nf_layers|5|
|epochs|500|
|split|0.8|
|batch_size|64|
|l2_reg|0.0001|
|learning_rate|0.001|
|random_state|42|

### PCC

|Parameter|Value|
|---|---|
|n_components|default|
|n_selected_components|default|
|whiten|default|
|svd_solver|auto|
|tol|default|
|max_iter|default|
|random_state|42|

### PCI

|Parameter|Value|
|---|---|
|window_size|0.5 dataset period size|
|thresholding_p|0.05|
|random_state|42|

### PS-SVM

|Parameter|Value|
|---|---|
|embed_dim_range|[0.5, 1.0, 1.5] * dataset period size|
|project_phasespace|False|
|nu|0.5|
|kernel|rbf|
|gamma|None|
|degree|3|
|coef0|0.0|
|tol|0.001|
|random_state|42|

### PST

|Parameter|Value|
|---|---|
|window_size|1.0 dataset period size|
|max_depth|4|
|n_min|1|
|y_min|default|
|n_bins|5|
|sim|SIMn|
|random_state|42|

### RBForest

|Parameter|Value|
|---|---|
|train_window_size|500|
|n_estimators|500|
|max_features_per_estimator|0.5|
|n_trees|500|
|max_features_method|auto|
|bootstrap|True|
|max_samples|None|
|random_state|42|
|verbose|0|
|n_jobs|1|
|max_depth|4|
|min_samples_split|2|
|min_samples_leaf|1|

### RobustPCA

|Parameter|Value|
|---|---|
|max_iter|default|
|random_state|42|

### S-H-ESD

|Parameter|Value|
|---|---|
|max_anomalies|dataset contamination|
|timestamp_unit|m|
|random_state|42|

### SAND

|Parameter|Value|
|---|---|
|anomaly_window_size|max anomaly length|
|n_clusters|50|
|n_init_train|10% of dataset length or until first anomaly|
|iter_batch_size|500|
|alpha|0.5|
|random_state|42|

### SARIMA

|Parameter|Value|
|---|---|
|train_window_size|500|
|prediction_window_size|50|
|max_lag|10% of dataset length|
|period|dataset period size|
|max_iter|default|
|exhaustive_search|False|
|n_jobs|1|
|random_state|42|

### Series2Graph

|Parameter|Value|
|---|---|
|window_size|1.0 dataset period size|
|query_window_size|1.5*window_size|
|rate|100|
|random_state|42|

### SR

|Parameter|Value|
|---|---|
|mag_window_size|40|
|score_window_size|40|
|window_size|1.0 dataset period size|
|random_state|42|

### SR-CNN

|Parameter|Value|
|---|---|
|window_size|1.5 dataset period size|
|random_state|42|
|step|64|
|num|10|
|learning_rate|0.001|
|epochs|500|
|batch_size|64|
|n_jobs|1|
|split|0.8|
|early_stopping_delta|0.05|
|early_stopping_patience|10|

### SSA

|Parameter|Value|
|---|---|
|ep|3|
|window_size|2.0 dataset period size|
|rf_method|alpha|
|alpha|0.2|
|random_state|42|

### STAMP

|Parameter|Value|
|---|---|
|anomaly_window_size|max anomaly length|
|exclusion_zone|0.5|
|verbose|0|
|n_jobs|1|
|random_state|42|

### STOMP

|Parameter|Value|
|---|---|
|anomaly_window_size|max anomaly length|
|exclusion_zone|0.5|
|verbose|0|
|n_jobs|1|
|random_state|42|

### Sub-Fast-MCD

|Parameter|Value|
|---|---|
|store_precision|True|
|support_fraction|default|
|random_state|42|

### Sub-IF

|Parameter|Value|
|---|---|
|window_size|1.0 dataset period size|
|n_trees|500|
|max_samples|None|
|max_features|1.0|
|bootstrap|false|
|random_state|42|
|verbose|0|
|n_jobs|1|

### Sub-LOF

|Parameter|Value|
|---|---|
|window_size|1.0 dataset period size|
|n_neighbors|50|
|leaf_size|20|
|distance_metric_order|2|
|n_jobs|1|
|random_state|42|

### TAnoGAN

|Parameter|Value|
|---|---|
|epochs|500|
|cuda|False|
|window_size|1.0 dataset period size|
|learning_rate|0.001|
|batch_size|64|
|n_jobs|1|
|random_state|42|
|early_stopping_patience|10|
|early_stopping_delta|0.05|
|split|0.8|
|iterations|25|

### TARZAN

|Parameter|Value|
|---|---|
|random_state|42|
|anomaly_window_size|max anomaly length|
|alphabet_size|4|

### Telemanom

|Parameter|Value|
|---|---|
|batch_size|64|
|smoothing_window_size|30|
|smoothing_perc|0.05|
|error_buffer|100|
|dropout|0.5|
|lstm_batch_size|64|
|epochs|500|
|split|0.8|
|early_stopping_patience|10|
|early_stopping_delta|0.05|
|window_size|1.5 dataset period size|
|prediction_window_size|50|
|p|0.17|
|random_state|42|

### Torsk

|Parameter|Value|
|---|---|
|input_map_size|100|
|input_map_scale|0.125|
|context_window_size|10|
|train_window_size|100|
|prediction_window_size|5|
|transient_window_size|20% of train_window_size|
|spectral_radius|2.0|
|density|0.01|
|reservoir_representation|sparse|
|imed_loss|False|
|train_method|pinv_svd|
|tikhonov_beta|None|
|verbose|0|
|scoring_small_window_size|10|
|scoring_large_window_size|100|
|random_state|42|

### Triple ES

|Parameter|Value|
|---|---|
|train_window_size|500|
|period|dataset period size|
|trend|add|
|seasonal|add|
|random_state|42|

### TSBitmap

|Parameter|Value|
|---|---|
|feature_window_size|500|
|lead_window_size|200|
|lag_window_size|500|
|alphabet_size|4|
|level_size|2|
|compression_ratio|1|
|random_state|42|

### VALMOD

|Parameter|Value|
|---|---|
|min_anomaly_window_size|1.0 dataset period size|
|max_anomaly_window_size|2.0 dataset period size|
|heap_size|50|
|exclusion_zone|0.5|
|verbose|0|
|random_state|42|
