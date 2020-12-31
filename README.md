# Spacy
``vocab``

``nlp.vocab``

``doc``

``Tokenizer``

`Matcher`
``from spacy.matcher import Matcher

matcher = Matcher(nlp.vocab)
pattern = [{"LOWER": "hello"}, {"LOWER": "world"}]
matcher.add("HelloWorld", None, pattern)
doc = nlp("hello world!")
matches = matcher(doc)``
