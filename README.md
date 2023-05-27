# Cat-meow-classification
<img src="https://raw.githubusercontent.com/colinbrandonpierce/Cat-meow-classification/main/Meow_cat_-_Mdebona.jpg" width="360" height="270"/>
<!-- {{Information |Description={{en|Shu Shu Lynn, ChubeLyn}} |Source=Transferred from [http://en.wikipedia.org en.wikipedia] |Date=2007-12-04 (original upload date) |Author=Original uploader was Mdebona at [http://en.wikipedia.org en.wiki-->
<hr>
<b>PROBLEM</b> <br>
What is your cat saying? Many cat owners feel like they know what their cat is saying. But could understanding cat meows be done in a data-based manner? This notebook attempts to do this on a dataset of cat meow audio files captured in one of three contexts: while being brushed, while isolated, or when waiting for food. <br><br>
Dataset: CatMeows: A Publicly-Available Dataset of Cat Vocalizations (https://zenodo.org/record/4008297)
<br><br>

<b>APPROACH</b> <br>
A standard approach to understand an audio file is to analyze its spectrogram, which provides the sounds frequencies and intensities over time. Training on the entirety of a cat meow spectrogram is computationally intensive, so an algorithm [1] was developed to extract the dominant harmonic as an approximation of the cat meow. Training was done on the loudest frequency, the max power of the meow, and the meow's length.
<br><br>
<img src="https://raw.githubusercontent.com/colinbrandonpierce/Cat-meow-classification/main/cat-harmonics.jpg" width="360" height="270"/>

<b>RESULTS</b><br>
Many of the audio files were poorly captured and did not display clear harmonics as they should. Plotting our features showed no clear patterns, except perhaps that cats sometimes meow louder when isolated. All cats have different psychologies and can have similar meows in different situations, so a different approach is likely necessary to tackle this problem.

<img src="https://raw.githubusercontent.com/colinbrandonpierce/Cat-meow-classification/main/3plot-features.png" width="360" height="340"/>

[1] The algorithm recursively crawls neighbors starting from the loudest frequency in the spectrogram matrix. The assumption is that a meow can be understood with only the loudest harmonic.


