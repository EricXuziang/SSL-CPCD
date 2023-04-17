## SSL-CPCD: Self-supervised learning with composite pretext-class discrimination loss for improved generalisability in endoscopic image analaysis

 ### Dataset details
 We explored three different datasets for our experiments on endoscopic image analysis as listed below:
 
 [LMIUC](https://zenodo.org/record/5827695#.ZD1Xsy_MIeY)
 
 [Kvasir-SEG](https://datasets.simula.no/kvasir-seg/)
 
 [CVC-ClinicDB](https://www.kaggle.com/datasets/balraj98/cvcclinicdb)
 
 In-house data (To be released!!!)
 
 ### Training, test and generalisation scripts 
 
 #### 1. Training for SSL-CPCD:
  <pre><code>
  cd ./SSL-CPCD
  python SSLCPCD_train.py
  </code></pre>
  ####  2. Training for downstream task:
  <pre><code>
  cd ./scriptDownstreamTaskTraining
  sh SSL_CPCD_finetune_UC_classification_train.sh
  sh SSL_CPCD_finetune_polyp_detection_train.sh
  sh SSL_CPCD_finetune_polyp_segmentation_train.sh
  </code></pre>
  ####  3. Test for each SSL-CPCD tasks
  <pre><code>
  cd ./SSL-CPCD_test
  python SSLCPCD_test.py
  </code></pre>
  #### 4. Test for each SSL-CPCD tasks (on unseen center)
  <pre><code>
  cd ./SSL-CPCD_test_generalisation
  python SSLCPCD_test_generalisation.py
  </code></pre>
