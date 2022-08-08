# Cat-meow-classification
<img src="https://raw.githubusercontent.com/colinbrandonpierce/Cat-meow-classification/main/Meow_cat_-_Mdebona.jpg" width="360" height="270"/>
<!-- {{Information |Description={{en|Shu Shu Lynn, ChubeLyn}} |Source=Transferred from [http://en.wikipedia.org en.wikipedia] |Date=2007-12-04 (original upload date) |Author=Original uploader was Mdebona at [http://en.wikipedia.org en.wiki-->
<hr>
<b>PROBLEM</b> <br>
What is your cat saying? A cat owner knows that there are roughly a finite number of meows per context. Could these be classified accurately in a data-based manner? This notebook attempts to do this with audio analysis and machine learning on recorded cat meows in well-defined contexts. <br><br>
Dataset: CatMeows: A Publicly-Available Dataset of Cat Vocalizations (https://zenodo.org/record/4008297)
<br><br>

<b>APPROACH</b> <br>
Audio recordings are often contained as a .wav file. A standard approach to understand an audio file is to see its spectrogram, which provides the waveform's frequencies and intensities over time. Training on the entirety of a cat meow spectrogram is too computationally intensive, so an algorithm [1] was develop to extract an approximation of the cat meow, to which training was done on the loudest frequency and the meow's length.
<br><br>
<img src="https://raw.githubusercontent.com/colinbrandonpierce/Cat-meow-classification/main/cat-harmonics.jpg" width="360" height="270"/>

<b>RESULTS</b><br>
KNN was able to obtain ~70% accuracy.

<img src="https://raw.githubusercontent.com/colinbrandonpierce/Cat-meow-classification/main/meow-space.jpg" width="360" height="270"/>

[1] The algorithm recursively crawls neighbors starting from the loudest frequency in the spectrogram matrix. The assumption is that a meow can be understood with only the loudest harmonic.


