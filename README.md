
<h1>The major objectives of this paper are as listed below:</h1>
<ul>
<li>To generate word-based features by analyzing frequently appearing words of email’s subjects and contents.</li>
<li>To generate link-based features by examining the URL links embedded in an email.</li>
<li>To generate the readability-based features using eight well-known readability algorithms and applying them to discriminate the text contents of phishing emails and legitimate emails.</li>
<li>To search the optimum features set using Pearson cor- relation algorithm (PCC) with binary search as well as the sequential forward search algorithm.</li>
<li>To verify the best features set by comparing with other feature selection algorithms on the basis of time, accu- racy and number of features.</li>
<li>To justify the method by comparing the results with the existing approaches.</li>
  </ul
  
  
<h2>Features from Hyperlinks</h2>
  
<ul>
  <li>has http</li>
  <li>has hypen</li>
  <li>num of subdomins</li>
  <li>has ipaddress</li>
  </ul>


<h2>Features from Readability Algorithms</h2>
<ul>
  <li>Automated Readability Index</li>
  <li>Coleman Liau Index</li>
  <li>Flesch–Kincaid Readability Test</li>
  <li>Gunning Fog Index</li>
  <li>SMOG Index</li>
  <li>LIX Readability Score</li>
  </ul>
  
  <h2>Pearson Correlation Algorithm (PCC)</h2>
  This paper has employed primarily Pearson correlation algo- rithm (PCC) to rank the features. It measures the linear corre- lation between two features. It assesses three classes of correlation: positive linear correlation is considered as 1, no linear correlation is 0, and negative linear correlation is −1.
  Assume X = {x1 , x2 , ... xn } and Y = {y1 , y2 , ... yn } are two sets of features. The PCC is defined by 𝜌, and equation is shown in (10).

        𝜌(X, Y) = cov(X, Y)/ 𝜎X, 𝜎Y
  
  
  
  
