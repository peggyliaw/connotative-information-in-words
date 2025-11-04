# connotative-information-in-words
Comparing human ratings on words' emotional aspects vs. emotion scores from embeddings (based on statistical co-occurrence)

### background

This project is inspired by Grand et al. (2018): https://arxiv.org/pdf/1802.01241. They used a technique called semantic projection to explore whether word embeddings contain context-dependent information. To do this, they constructed various semantic dimensions like size ("small" to "big"), intelligence ("dumb" to "smart"), danger ("safe" to "dangerous"), etc. Then they projected groups of words onto these dimensions to see whether word embeddings demonstrate knowledge about context-depndent meanings.

It is widely believed that words contain connotative meanings, even when they are non-emotional words. Traditionally, research on emotion has mainly used the framework by Osgood et al. (1957), who proposed three dimensions for emotion: valence (negative to positive), arousal (calm to exciting), and dominance (weak to strong). A traditional way of quantifying emotional information in words is to ask participants to rate how the word feels to them (e.g., Warriner et al., 2013). Researchers use these ratings to further examine how emotional meanings in words can impact word processing like lexical decision time.

### goal

Are people's ratings of how words feel to them the same as how these words are used in relation to emotional words? That is, does the word rating task on emotions sufficiently capture emotional aspects of words?

This project answers this question. I obtained valence, arousal, and dominance scores from word2vec-google-news-300. Then I correlated these scores with human ratings from Warriner et al. (2013): https://doi.org/10.3758/s13428-012-0314-x

### findings

The results are what would be expected based on existing literature: valence ratings are consistent, arousal are ok-ish, and dominance are the least reliable. This could probably tell us that the emotions people feel about a word may not be the same as how the words are used. However, there is not enough evidence to say embedding scores are the "true values". There may be other things going on in a person when they judge a word. Next steps could be to control for other psycholinguistic variables like frequency, concreteness, imaginability, etc. and see how well human ratings can predict embedding scores.
