# SSL-CPCD: Self-supervised learning with composite pretext-class discrimination loss for improved generalisability in endoscopic image analaysis
  ## 1. Abstract
  ## 2. Training for SSL-CPCD:
  <pre><code>cd ./SSL-CPCD
             python SSLCPCD_train.py

  </code></pre>
  ## 3. Training for downstream task:
  <pre><code>cd ./scriptDownstreamTaskTraining
              sh SSL_CPCD_finetune_UC_classification_train.sh
              sh SSL_CPCD_finetune_polyp_detection_train.sh
              sh SSL_CPCD_finetune_polyp_segmentation_train.sh
             

  </code></pre>
