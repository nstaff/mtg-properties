# Magic The Gathering properties

This is a collection of RegExp values that allow for fast search on properties instead of text.

having properties be readable by machines give you the ability to create awesome integrations and apps.
Look at this graph we can build by linking properties [Magic Graph](http://magic.jocolina.com)

## Explanation
Every ability has a name (only 3 for now) and given RegExps.
These regular expressions are built in two ways:
* One for the actions needed by the card to trigger (`needs`)
* The other for the abilities the card is able to trigger (`does`)


## Contributing
To contribute, fork this repo and add all the properties you want with all needed RegExp.
You can test them on MTG JSON files ;) 

You can then open a Pull Request that i'll review as fast as I can (but won't run any tests).

To contribute, follow the following format
```json
{
	"name": "life_gain",
	"reg": {
		"does": "gain( \\d)? life",
		"needs": "gained life"
	},
	"description": "Player gains life, or executed whenever player gains life"
},
```