
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
