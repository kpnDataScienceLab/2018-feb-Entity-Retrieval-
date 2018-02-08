# Wikipedia Entity Retrival using Deep Networks

My plan is to use the *wikipedia categories* section as **queries**, and the wikipedia articles as **entities**. I have already parsed these into a big json file: 

```json
{
	"20th-century american engineers": [
	        "<dbpedia:Albert_Einstein>",
	        "<dbpedia:Nikola_Tesla>",
	        "<dbpedia:Wernher_von_Braun>",
	        "<dbpedia:Wright_brothers>",
	        "<dbpedia:Jack_Parsons_(rocket_engineer)>",
	        "<dbpedia:Harold_H._Seward>",
	        "<dbpedia:Scott_Werndorfer>",
	        "<dbpedia:Willibald_Peter_Prasthofer>",
	        "<dbpedia:Nils_F._Ambursen>",
	        "<dbpedia:Zara_Cisco_Brough>",
	        "<dbpedia:Melvin_J._Glimcher>"
	    ],
	    ....
}
```

So the entries to be retrieved for the query "20th-century american engineers" is all the above listed entities. We can use **nordlys API** to retrieve the entities abstracts like this: `http://api.nordlys.cc/ec/lookup_id/<dbpedia:Albert_Einstein>`. 


For the model I plan to use the deep networks introduced in [this paper](https://arxiv.org/abs/1704.08803). 


