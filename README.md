cws
===

##Chinese Word Segmentation - Overview
In languages such as English or French, words are typically separated by spaces, making sentence tokenization simple. However, in Chinese (and Japanese Kanji), the written language consists of characters that are not delimited, making word tokenization difficult. A given character may have an independent meaning as a word, and a separate meaning when grouped with other characters. For instance, the character 中 means 'middle', 将 means 'will', and when combined, 中将 means 'lieutenant general'. This can lead to ambiguities when attempting to segment and translate a sentence, since depending on the context, the correct translation of 中将 may be 'middle will', while in another context it may be 'lieutenant general'. As a result, Chinese word segmentation (CWS) becomes an important step when translating from Chinese.

To further illustrate with an English example, consider the character sequence “ISHIP”. This sequence could either be segmented as “IS HIP” or “I SHIP”, leading to the two different sentences “I will save all the code that I ship” and “I will save all the code that is hip”. 

The CWS problem is to transform an input character sequence S without spaces to a sequence Sseg, where Ssegcontains spaces between word segments. Numerous methods have been developed or applied to the problem, such as the Compression-Based algorithm, Conditional Random Fields, and the Maximum Entropy Model. 

##This Project
```script```: a perl script that computes the average of Recall, Precision, and F-Measure, as well as various statistics for a given prediction set. It is a slightly modified version of the script used for the SIGHAN Bakeoff competition.
