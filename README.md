<h1 align="center">"More Than Words": Linking Music Preferences and Moral Values through Lyrics</h1>
<div align="center">

This directory contains the lyrics data and the code for lyrical feature modeling from our paper that have been accepted to the 23rd International Society
for Music Information Retrieval Conference ([ISMIR 2022](https://ismir2022.ismir.net/)).
Due to the privacy issues here we share only the partial implementation discussed in our paper. 

## Install:

To reuse this repo, install the requested libraries  
```bash
pip install -r requirements.txt
```
## Data:
In the data folder you can find all the .csv files that contain song lyrics and the features scores. Also, we have added the best obtained LDA model file the Topic Visualisation (.html) file. 

## Implementation:
The `notebooks` directiory contains the jupiter scripts for obtaining lyrics features: 
sentiment analysis with ([VADER](https://github.com/cjhutto/vaderSentiment)), emotion associations with ([NRC lexicon](https://saifmohammad.com/WebPages/AccessResource.htm)), moral scores with ([MoralStrength](\https://github.com/oaraque/moral-foundations)) lexicon) and modell lyrics topics using LDA topic modelling.
Whereas, the `py_scripts` folder contains the python code for lyrics scraping using ([Genius API](https://docs.genius.com/)) cleaning and preprocessing and language detection using ([spaCy](https://spacy.io/)).

## Citation
```bibtex
@article{preniqi2022morals,
    title={{"More Than Words": Linking Music Preferences and Moral Values through Lyrics}},
    author={Preniqi, Vjosa and Kalimeri, Kyriaki and Saitis, Charalampos},
    journal={Proceedings of the 23rd International Society for Music Information Retrieval Conference},
    year={2022}
}
```