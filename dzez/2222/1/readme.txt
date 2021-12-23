This directory is user 2222's personal transclusion of 1111's article.  1.json has the EDL for the full transclusion of version 9 of the article.

"richlink":"2222/1/1" = the tumbler for this rich link (points to this 1.json)
,"home":"2222/0" = the tumbler for the dimension list of this user/hyperdrive
,"from":"1111/2/9/1/0" = the starting point of the transclusion = first byte of 1111's document
,"to":"1111/2/9/1/5393" = the ending point of the transclusion = last byte of 1111's document
,"type":"2222/0/2/1" = zzcell that has the type of this rich link:	{"value":"transclusion",

Note: the mechanism for identifying byte ranges of a file is open for comments.
With the notation above, if there do not exist subdirectories named "0" or "5393"
The tumbler can be interpreted as a byte position.
An alternative can be to have both "from" and "to" point to "1111/2/9/1" which would 
indicate the entire contents of the 1.md file in 1111/2/9.