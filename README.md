<h1 align="center">"More Than Words": Linking Music Preferences and Moral Values Through Lyrics</h1>
<div align="center">
</div>

This directory contains the lyrics data and the code for lyrical feature modeling from our paper that have been accepted to the 23rd International Society
for Music Information Retrieval Conference ([ISMIR 2022](https://ismir2022.ismir.net/)).
Due to the privacy issues here we share only the partial implementation discussed in our paper. 

## Install:

To reuse this repo, install the requested libraries  
```bash
pip install -r requirements.txt
```
## Data:
In this repo, we share artists' lyrics and the content features we have extracted. The artists were selected based on the artist page names liked on Facebook by the _LikeYouth_ participants (this is the main dataset we use, please read the paper for more info about this data).
In the data directory, we have added  the .csv file of artist page names and the directions to download artists' lyrics and features scores. Also, we have provided the best obtained LDA model file and the topic visualisation (.html) file. 

## Implementation:
The `notebooks` directory contains the Jupyter scripts for obtaining lyrics features: 
sentiment analysis with [VADER](https://github.com/cjhutto/vaderSentiment), emotion associations with 
[NRC lexicon](https://saifmohammad.com/WebPages/AccessResource.htm), moral scores with [MoralStrength](\https://github.com/oaraque/moral-foundations)) lexicon and lyrics topics using LDA topic modeling.
Whereas, the `py_scripts` folder contains the python code for lyrics scraping using [Genius API](https://docs.genius.com/) cleaning and preprocessing and language detection using [spaCy](https://spacy.io/).


<!-- ## Citation
```bibtex
@article{preniqi2022lyrics_and_morals,
    title={{"More Than Words": Linking Music Preferences and Moral Values through Lyrics}},
    author={Preniqi, Vjosa and Kalimeri, Kyriaki and Saitis, Charalampos},
    journal={Proceedings of the 23rd International Society for Music Information Retrieval Conference},
    year={2022}
}
```
 -->
