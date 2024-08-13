**Text Analysis using NLP**

**Objective**

The objective of this project is to apply Natural Language Processing (NLP) techniques to perform comprehensive text analysis. The analysis covers a variety of metrics including sentiment analysis, readability, word count, syllable count, personal pronouns, and more.

**Table of Contents**

Sentimental Analysis

1.1 Cleaning using Stop Words Lists

1.2 Creating a Dictionary of Positive and Negative Words

1.3 Extracting Derived Variables

Analysis of Readability

Average Number of Words Per Sentence

Complex Word Count

Word Count

Syllable Count Per Word

Personal Pronouns

Average Word Length

**Sentimental Analysis**

Sentimental analysis is the process of determining whether a piece of text is positive, negative, or neutral. This project is specifically designed to analyze financial texts. The process involves:

**Cleaning using Stop Words Lists**

The text is cleaned using predefined Stop Words Lists to remove irrelevant words, ensuring accurate sentiment analysis.

**Creating a Dictionary of Positive and Negative Words**

A master dictionary is used to create lists of positive and negative words. Words from the Stop Words Lists are excluded from this dictionary.

**Extracting Derived Variables**

Positive Score: Calculated by assigning a +1 value for each word found in the Positive Dictionary.
Negative Score: Calculated by assigning a -1 value for each word found in the Negative Dictionary. The score is multiplied by -1 to ensure it's positive.
Polarity Score: Determines if the text is positive or negative using the formula:
Polarity Score = (Positive Score – Negative Score) / (Positive Score + Negative Score + 0.000001)
Range: -1 to +1.
Subjectivity Score: Determines if the text is objective or subjective using the formula:
Subjectivity Score = (Positive Score + Negative Score) / (Total Words after cleaning + 0.000001)
Range: 0 to +1.
Readability Analysis
Readability is assessed using the Gunning Fog Index, which is calculated as:
Fog Index = 0.4 * (Average Sentence Length + Percentage of Complex Words)

Additional Metrics

**Average Number of Words Per Sentence**

Complex Word Count: Words with more than two syllables.
Word Count: Total cleaned words after removing stop words and punctuations.
Syllable Count Per Word: Number of syllables per word, with exceptions like words ending in "es" or "ed."
Personal Pronouns: Count of personal pronouns using regex, excluding terms like "US" referring to the country.
Average Word Length: Sum of characters per word divided by the total number of words.

This project provides a comprehensive toolkit for analyzing textual data, especially in the financial domain, by leveraging NLP techniques.
