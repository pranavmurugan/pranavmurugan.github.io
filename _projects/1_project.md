---
layout: page
title: NLP for Symptom Detection
description: Natural Language Processing for Symptom Detection in Unstructured Provider-Patient Conversation -- MIT Machine Learning in Healthcare Semester Project
img: assets/img/1_project_img4.png
importance: 1
category: MIT
---

<h4>Full text: <a href="/assets/pdf/6_871final_paper.pdf" target="_blank" rel="noopener noreferrer"><i class="fas fa-file-pdf"></i></a></h4>
<br/>
A summary is shown below.
<br/><br/>
<h5>Objective</h5>
We identify symptom-related conversation segments in physician-patient dialogue using natural language processing (NLP) techniques, with the goal of developing an automated pipeline for symptom detection in unstructured clinical conversation. Our work helps address the high symptom burden placed on patients, improving care satisfaction and decreasing healthcare costs.
<br/><br/>
<h5>Dataset Overview</h5>
- Turn-level conversation data between patients and their healthcare provides 
- Roughly 79,000 turns spanning over 181 unique conversations and 94 unique patients 
- Around 13% of the turns are symptom-related
<br/><br/>
<h5>Model Comparison</h5>
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/1_project_img1.png" title="Figure 1" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<br/><br/>
<h5>Results</h5>
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/1_project_img2.png" title="Table 1" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Precision-recall curve for each method tested. Right: Receiver-Operator Characteristic (ROC) curves for each method. The dashed gray line indicates the curve for a perfectly random classifier. The associated AUROC for each of these curves can be found in Table 1. Error bars show the 95% confidence interval and were estimated with a bootstrap method using 250 resamples per threshold value.
</div>
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/1_project_img3.png" title="Figure 2" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Quantitative metrics for each model on the non-preprocessed data. 
</div>
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/1_project_img4.png" title="Figure 3" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    SHAP Plot using XGBoost.
</div>
<br/><br/>
<h5>Takeaways</h5>
- Transformer-based BERT model performed the best, but LSTM is second best and is less computationally-intensive
- BioBERT performed poorly, suggesting conventional NLP models are sufficient
- Bag-of-words models are very interpretable; next steps may focus on the interpretation of the deep learning models
- Future goal is to incorporate symptom detection in an automatic pipeline during patient care
<br/><br/>
<h5>Full text: <a href="assets/pdf/6_871final_paper" target="_blank" rel="noopener noreferrer"><i class="fas fa-file-pdf"></i></a></h5>
<h5>Github: <a href="https://github.com/pmuruga/symptom-detection" title="GitHub"><i class="fab fa-github"></i></a></h5>
<br/>