Each numbered directory defines a dimension.
The json files in this directory provide metadata for the corresponding dimension.
For this user
1 = d.mystuff
2 = d.linktype
3 = d.correspondence

Tumblers:
0/1 = 1.json containing "dimname": "d.mystuff"
0/1/n = json files in 2222/0/1: cells created whose first link is on d.mystuff
0/2 = 2.json containing "dimname":"d.linktype"
0/2/1 = 1.json in 2222/0/2 containing zzcell: "value":"transclusion"
0/2/2 = 2.json in 2222/0/2 containing zzcell: "value":"comment"


