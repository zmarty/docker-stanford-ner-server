# Stanford Named Entity Recognizer (NER) Server Docker Image

Docker image that contains the **[Stanford Named Entity Recognizer (NER) Server](http://nlp.stanford.edu/software/CRF-NER.shtml)**.

**What is Stanford Named Entity Recognizer (NER)**

From [official website](http://nlp.stanford.edu/software/CRF-NER.shtml): *Stanford NER is a Java implementation of a Named Entity Recognizer. Named Entity Recognition (NER) labels sequences of words in a text which are the names of things, such as person and company names, or gene and protein names. It comes with well-engineered feature extractors for Named Entity Recognition, and many options for defining feature extractors.*

**What is Stanford NER Server?**

From [class documentation](http://nlp.stanford.edu/nlp/javadoc/javanlp/edu/stanford/nlp/ie/NERServer.html): *A named-entity recognizer server for Stanford's NER. Runs on a socket and waits for text to annotate and returns the annotated text. (Internally, it uses the classifyString() method on a classifier, which can be either the default CRFClassifier which is serialized inside the jar file from which it is called, or another classifier which is passed as an argument to the main method.*

**How to run it**

```
docker run -it --rm zmarty/stanford-ner-server
```

If you are new to Docker, please note that due to the rm command line argument above all your file changes within the container will be lost.
