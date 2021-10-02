# DataResrival-BM25

Based on the direct change of DataRetrival-VectorSpace, some unnecessary programs have been deleted to improve the retrieval time.

In the calculation of BM25, there are many parameters that need to be set. 

When writing a program, I found that if there are many words containing query in the document when calculating the IDF of the document. The value in Log will be a score less than 1 and the Log value will be a negative value.
So the Log value add 1 to avoid scores are less than 1.
After that the log value is positive, there is a better comparison result.
