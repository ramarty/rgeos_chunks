# rgeos functions in chunks
Sometimes it is memory intensive to implement an rgeos function on a large dataset, but it takes a while to implement the function row by row. A faster approach is to implement the function in "chunks." For example, it is memory intensive to calculate the distance from 3,000,000 points to a line segment. As a faster approach, we can break the points dataset into chunks of 10,000 points, and calculate the distance in the chunks.

Functions Converted
* gBuffer --> gBuffer_chunks
* gDistance --> gDistance_chunks

