# Spacy
``vocab``

``nlp.vocab``

``doc``

``Tokenizer``

`Matcher`

```from spacy.matcher import Matcher
matcher = Matcher(nlp.vocab)
pattern = [{"LOWER": "hello"}, {"LOWER": "world"}]
matcher.add("HelloWorld", None, pattern)
doc = nlp("hello world!")
matches = matcher(doc)```


`Pharasematcher`

```from spacy.matcher import PhraseMatcher
matcher = PhraseMatcher(nlp.vocab)
matcher.add("OBAMA", None, nlp("Barack Obama"))
doc = nlp("Barack Obama lifts America one last time in emotional farewell")
matches = matcher(doc)```
