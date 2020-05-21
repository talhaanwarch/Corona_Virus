# Corona_Virus
## Diagnosed using X-ray and CT-scan
Two different dataset has been tried. 
* X-ray dataset
* CT-scan dataset
# Results using Chest Xray dataset
There are three classes in this dataset
* covid
* normal
* pneumonia

No seprate test holdout dataset is used. Instead 5 fold cross validation technique is used. The dataset is taken from [tawsifur/COVID-19-Chest-X-ray-Detection](https://github.com/tawsifur/COVID-19-Chest-X-ray-Detection) github repo. The author achieved an F1-score of 0.983, where as we got an F1-score of 0.981.
<table>
<thead>
  <tr>
    <th></th>
    <th>Precision</th>
    <th>Recall</th>
    <th>F1-score</th>
    <th>Accuracy</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Fold 1</td>
    <td>0.99</td>
    <td>0.98</td>
    <td>0.98</td>
    <td>0.98</td>
  </tr>
  <tr>
    <td>Fold 2</td>
    <td>0.99</td>
    <td>0.98</td>
    <td>0.99</td>
    <td>0.98</td>
  </tr>
  <tr>
    <td>Fold 3</td>
    <td>0.97</td>
    <td>0.98</td>
    <td>0.98</td>
    <td>0.97</td>
  </tr>
  <tr>
    <td>Fold 4</td>
    <td>0.98</td>
    <td>0.98</td>
    <td>0.98</td>
    <td>0.97</td>
  </tr>
  <tr>
    <td>Fold 5</td>
    <td>0.98</td>
    <td>0.98</td>
    <td>0.98</td>
    <td>0.97</td>
  </tr>
</tbody>
</table>


We achieved an F1 score of <strong>0.98</strong>. Result can be reproduce through this [notebook](https://github.com/talhaanwarch/Corona_Virus/blob/master/notebooks/Corona_aug.ipynb)

In order to download data in [notebook](https://github.com/talhaanwarch/Corona_Virus/blob/master/notebooks/Corona_aug.ipynb) you need to provide it a kaggle API. Go to kaggle.com, click on my account and then go to API section. Click on create new API token. It will download a file , *kaggle.json* . upload this *kaggle.json*  to *content* folder of colab. And run the whole notebook.
## Result using CT-scan dataset  
Dataset is taken from [github.com/UCSD-AI4H/COVID-CT](https://github.com/UCSD-AI4H/COVID-CT) repo, where author achieved an F1-score of 0.85.  
<strong>All CT-scan related files are in CT-scan folder</strong>  
Here i study effect of learning rate on model performance.  
<table>
<thead>
  <tr>
    <th></th>
    <th>Plateau LR</th>
    <th>Cyclic LR</th>
    <th>Constant LR</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Macro Average Precision</td>
    <td>0.90</td>
    <td>0.89</td>
    <td>0.85</td>
  </tr>
  <tr>
    <td>Macro Average Recall</td>
    <td>0.89</td>
    <td>0.86</td>
    <td>0.82</td>
  </tr>
  <tr>
    <td>Macro Average F1 Score</td>
    <td>0.90</td>
    <td>0.86</td>
    <td>0.82</td>
  </tr>
  <tr>
    <td>Accuracy</td>
    <td>0.90</td>
    <td>0.86</td>
    <td>0.86</td>
  </tr>
  <tr>
    <td>AUC score</td>
    <td>0.90</td>
    <td>0.86</td>
    <td>0.82</td>
  </tr>
</tbody>
</table>

Jeremy Kohn has compiled all image based diagnostic of coronavirus at one place. Do check his repo [github.com/jeremykohn/rid-covid](https://github.com/jeremykohn/rid-covid)

# PAPER citation
Anwar, Talha; Zakir, Seemab (2020): Deep learning based diagnosis of COVID-19 using chest CT-scan images. TechRxiv. Preprint. https://doi.org/10.36227/techrxiv.12328061.v1

