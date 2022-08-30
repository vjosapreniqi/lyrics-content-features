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
In this directory, we have added the initial `artist page names` that were liked by the _LikeYouth_ (read more about this data [here](https://www.isi.it/media/255)) participants on Facebook.  Also, we have provided the best obtained LDA model file and the topic visualisation (.html) file. 

To get access to artists' lyrics and the lyrics' content features, please download the data as a `zip file` from the [Lyrics_annotated_data](https://osf.io/kftqr/files/osfstorage) hosted in the [OSF](https://osf.io/kftqr/files/osfstorage) directory. When cloning/downloading the repo, add the `.csv files` into this directory to re-run the experiments we described. When using the initial `artist_lyrics_initial_dt.csv` and re-running the scripts we have provided here, you should be able to reproduce the `artist_lyrics_annotated_vader_nrc_moralStrength_lda_final_dt.csv` we shared [here](https://osf.io/kftqr/files/osfstorage).

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
