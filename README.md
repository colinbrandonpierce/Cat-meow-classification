# Cat-meow-classification
Cat meow classifier

<img src="https://raw.githubusercontent.com/colinbrandonpierce/Cat-meow-classification/main/meow-harmonics.png" width="300" height="300" />
<hr>
<b>PROBLEM</b>
What is your cat saying when it is home alone? This problem can be tackled with audio analysis and machine learning.
Dataset:...
<br><br>

<b>APPROACH</b>
<img src="https://raw.githubusercontent.com/colinbrandonpierce/Cat-meow-classification/main/meow-extraction.png" width="300" height="300" />
Training on the entirety of a cat meow spectrogram is too intensive. An algorithm was develop to extract an approximation of the cat meow, to which training was done on the loudest frequency and the meow's length.

<b>RESULTS</b>
<img src="https://raw.githubusercontent.com/colinbrandonpierce/Cat-meow-classification/main/meow-space.png" width="300" height="300" />
Using KNN, was able to obtain ~70% accuracy training on just two columns.


