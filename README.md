# NLP
## Text processing Level 1:
### Tokenization:
- Tokenization involves breaking down text into smaller units called tokens, which can be words, phrases, sentences, or characters.
- Tokenization is a crucial step in NLP because it forms the foundation for various language processing tasks, such as text classification, named entity recognition, machine translation, and sentiment analysis.
- Here are a few examples of tokenization:
  1. Word Tokenization: In this type of tokenization, the input text is divided into individual words. For example, the sentence "Tokenization is important for NLP." would be tokenized into: ["Tokenization", "is", "important", "for", "NLP", "."].
  2. Sentence Tokenization: In this case, the text is divided into individual sentences. For instance, the paragraph "Tokenization is important. It helps in breaking down text." would be tokenized into: ["Tokenization is important.", "It helps in breaking down text."].
  3. Character Tokenization: The text is broken down into individual characters. For example, the word "Hello" would be tokenized into: ["H", "e", "l", "l", "o"].
  4. Subword Tokenization: This approach breaks down words into smaller meaningful units, such as prefixes, suffixes, or stems. For instance, the word "unhappiness" might be tokenized into: ["un", "happiness"].

### Stemming and Lemmetization
- Process of reducing infected words to their word stem.
- Difference between Stemming and Lemmetization:
  - Stemming may not give meaningful word representation, where as Lemmetization always give meaningful word representation.
  - Stemming takes less time for finding word representation than Lemmetization.
  - Stemming can be used in application where meaningful represention are neccesary in the output of the application such as positive/negetive sentiment analysis and gmail spam classifier. Lemmetization are used in application where meaningful representaion are neccesary in the output of the application such as chabot, QA.
### Stop words

## Text Processing Level 2:
### Bag-Of-Words and Binary Bag-Of-Words
- It converts the sentences into the vector representations, as the machine understands the numeric values.
- In Bag-Of-words and Binary Bag-Of-Words, The histogram of corpus is calculated and sorted to descending order.
- Binary Bag-Of-Words uses 1/0 in vector representation if the word is present in sentence or not.
- Bag-Of-Words approach uses the frequency of the word in vector representation.
- The problem with these approach is they weighs all words the same weight.
### Term Frequency - Inverse Document Frequency (TF-IDF)
- Term Frequency = No of repeatation of the word / No of words in a sentence
- Inverse Document Frequency = log( No of sentences / No of sentences containing the word )
- The vector is calculated as TF*IDF for each word present ad rest are zeros.
### Word2Vec
- Drabacks of previous methods
  - In both BOW and TF-IDF, semantic information is not stored. TF-IDF gives importance to uncommon words.
  - There is definitly chance of overfitting.
- In this specific model, each word is basically represented as a vector of 32 or more dimension instead of a single number.
- Here, the semantic information and relation between different words is also preserved.
