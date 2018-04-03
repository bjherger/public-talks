# Meta

## Audience

Conferences

 - DefCon
 - BlackHat

People

 - Hacker types
 - Interest in security
 - Strong CS background
 - Probably weaker ML background
 - Strong bullshit filter
 - Probably traveling on their own dime
 - Possibly security professionals or training to be professionals

## Lit review

 - AWS Macie
 - Dumpmon & equivalents
 - Wifi crackers / dictionary attacks(?)

AWS Macie

 - Reviewing [product page](https://aws.amazon.com/macie/)
 - Unclear what PII is covered
 - Limited to S3
 - Uses ML

Dumpmon

 - Reviewing [blog post](http://raidersec.blogspot.com/2013/03/introducing-dumpmon-twitter-bot-that.html)
 - Strong connection to paste-sites
  - Pastebin, Pastie, Slexy, 
 - Looks for regular expressions

[PastebinLeaks](https://twitter.com/PastebinLeaks)

 - Wide variety of regex expressions

[WPA2 cracker](https://github.com/brannondorsey/wifi-cracking)

 - Uses underlying tools

[hashcat](https://github.com/hashcat/hashcat)

 - Can brute force by character set, word list, or combinations of wordlists
 - [Wordlist list](https://hashcat.net/forum/thread-1236.html)

# Submission

## Speaker

### Bio

Brendan Herger is a Machine Learning Engineer who has built Machine Learning & Natural Language Processing platforms for catch credit card fraud, insider threat, and legal document processing. He specializes in using Machine Learning for domains with adversarial elements and large unstructured data sets.

## Title

Beyond Regex: Using Deep Learning to find sensitive data in pastebins

## Track

## Abstract

Pastebins and large data dumps can contain troves of interesting fields, historically unstructured data has been mined using regular expressions, and pattern matching heuristics. However, deep learning approaches provide for a more robust approach to learning and extracting data these techniques can't capture, such as pattern-less formats (e.g. passwords, usernames, addresses). 

## Presentation outline

 - XKCD Comic
 - Introduction 
   - Background / setting context
   - Use cases
 - Historical approaches
   - Regex based
   - Pattern matching / boostrapping
   - Shortcomings
 - Machine Learning Approaches
   - Named entity recognition
   - Outlier detection (word level)
   - Deep learing classifier
   - Chacter level word embeddings
   - Auto-encoder
 - Recap
   - Intro / why
   - Historical / shortcomings
   - ML / strengths
 - Future work
   - Train on large data sets of compromised credentials
   - Segment by source document file type
   - Look for new data formats

## What new research, concept, technique, or approach is included in your submission that the audience has never seen before?

Using Deep Learning & Natural Language Processing to extract data fields from unstructured text data

## Takeaways

 - Valueable data can be extracted from unstructured text
 - The barrier to entry is relatively low

## So the Review Board is able to get a sense of your presentation style, do you have a video sample of any previous conference presentations?

https://www.youtube.com/watch?v=u72FD79tsxA
https://www.youtube.com/watch?v=J_D4QuXb81w
