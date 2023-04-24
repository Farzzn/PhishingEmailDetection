
<h2>The major objectives of this paper are as listed below:</h2>
<ul>
<li>To generate word-based features by analyzing frequently appearing words of email’s subjects and contents.</li>
<li>To generate link-based features by examining the URL links embedded in an email.</li>
<li>To generate the readability-based features using eight well-known readability algorithms and applying them to discriminate the text contents of phishing emails and legitimate emails.</li>
<li>To search the optimum features set using Pearson cor- relation algorithm (PCC) with binary search as well as the sequential forward search algorithm.</li>
<li>To verify the best features set by comparing with other feature selection algorithms on the basis of time, accu- racy and number of features.</li>
<li>To justify the method by comparing the results with the existing approaches.</li>
  </ul>
  
  
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
  This paper has employed primarily Pearson correlation algorithm (PCC) to rank the features. It measures the linear correlation between two features. It assesses three classes of correlation: positive linear correlation is considered as 1, no linear correlation is 0, and negative linear correlation is −1.
  Assume X = {x1 , x2 , ... xn } and Y = {y1 , y2 , ... yn } are two sets of features. The PCC is defined by 𝜌, and equation is shown in (10).

        𝜌(X, Y) = cov(X, Y)/ 𝜎X, 𝜎Y
        
        
        
 <h2>Binary Search Feature Selection (BSFS)</h2>
<p> Here I introduces a novel algorithm named binary search feature selection (BSFS) algorithm, which explores the best feature set with the least time and better accuracy. The binary search feature selection is inspired by the binary search algorithm which is shown in Algorithm 2. This algorithm initially selects half of the fea- tures from the feature’s corpus ((fa–fm)) where m denotes the midpoint that is half of the features; the accuracy is evaluated ( C ← Acc(S + x+)). If the accuracy is above the threshold value (the method used the same threshold value of sequential forward feature selection algorithm), then the method examines the  rst half of the midpoint and upgrades the threshold value with current accuracy and in the same way runs the algorithm. If the method is unable to ascertain the better accuracy than the threshold value, then the method investigates the adjacent half by assigning the midpoint with the initial point with the same threshold value.</p>
<h3>Binary Search Feature Selection Algorithm</h3>
BSFS(Fi ={f1,f2,...fn}) S ← ∅<br>
l ← size(Fi)<br>
a ← 0<br>
forl≥ado<br>
m ← div((a + l),2)<br>
x+ ← (fa to fm) <br>
C ← Acc(S + x+) <br>
if C ≤ Thld then<br>
S ← S + x+ <br>
a←m+1<br>
go to step 5<br>
else<br>
Thld ← C + S←S+x<br>
l←m−1<br>
go to step 5<br>
end if<br>
return Thld <br>
end for
  
