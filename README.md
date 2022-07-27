# Emotion Detection in Song Lyrics

Emotions play a fundamental role in songs, in such a way that an entire branch of psychology is devoted to understand the relationships between 
human affect and music. Emotions are also the center of attention of numerous sentiment analysis studies, concentrated in particular to the 
identification of them inside texts or facial expressions. This research focuses on detecting from song lyrics which are the feelings that a 
listener can experience, starting from understanding what is an emotion and in which way it is possible to represent it.

## Dataset

This research has been conducted on two datasets, one used for the learning phase and the other for the application one. 
During the first part of the analysis, the [EmoBank](https://github.com/JULIELab/EmoBank) dataset has been chosen in order to train the model.
The data consists in more than ten thousand observations, each of it representing a sentence and the corresponding values for the VAD scheme (valance, arousal, dominance); 
a subset of it has also been manually annotated with the Ekman’s six basic emotions.

For the application phase, the data has been retrieved using the Genius API from [genius.com](genius.com), a popular website collecting insights about music. 
For each of the five major music genres identified by the site (Rap, Pop, Country, R&B, Rock), the most popular 100 songs of all time have been retrieved, 
together with their respective lyrics.

## Technologies

* Language Processing: `nltk`, `spacy`, `gensim`
* Machine Learning: `tensorflow`, `keras`, `sklearn`

## References

* Ekman, P. (1992). An argument for basic emotions. In Cognition and Emotion (Vol. 6, Issues 3–4, pp. 169–200). Informa UK Limited. https://doi.org/10.1080/02699939208411068
* Mehrabian, A., & Russell, J. A. (1974). An approach to environmental psychology. The MIT Press.
* Buechel, S., & Hahn, U. (2018). Word Emotion Induction for Multiple Languages as a Deep Multi-Task Learning Problem. In Proceedings of the 2018 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long Papers). Proceedings of the 2018 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long Papers). Association for Computational Linguistics. https://doi.org/10.18653/v1/n18-1173
* Sven Buechel and Udo Hahn. 2017. EmoBank: Studying the Impact of Annotation Perspective and Representation Format on Dimensional Emotion Analysis. In EACL 2017 - Proceedings of the 15th Conference of the European Chapter of the Association for Computational Linguistics. Valencia, Spain, April 3-7, 2017. Volume 2, Short Papers, pages 578-585. Available: http://aclweb.org/anthology/E17-2092
* Sven Buechel and Udo Hahn. 2017. Readers vs. writers vs. texts: Coping with different perspectives of text understanding in emotion annotation. In LAW 2017 - Proceedings of the 11th Linguistic Annotation Workshop @ EACL 2017. Valencia, Spain, April 3, 2017, pages 1-12. Available: https://sigann.github.io/LAW-XI-2017/papers/LAW01.pdf
