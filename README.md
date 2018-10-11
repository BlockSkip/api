# api
API documentation to teach how to use BlockSkip API. All API endpoint need to be call by POST JSON. At free environment you don't need to pass key, signature and nonce and private key is not encrypted too.

http://blockskip:3040/free/createWallet

Request
{
	"asset":"xrp"
}

Response
{
    "asset": "XRP",
    "address": "rfmsbXWjB8qLudhzwy3johj8Pm9UBAFwWD",
    "privateKey": "U2FsdGVkX1+QFOocUjBv20aoGdjteJyLm3kHl46MV3cv6A9QAVS+8DcH9Ra2xh+Z"
}

http://blockskip:3040/free/getBalance

Request
{
	"asset":"etc",
	"address": "0xE91D422AB7CDf4558FF66365A23a5978F8BF9100",
	"confirmations": 1
}

Response
{
    "address": "0xE91D422AB7CDf4558FF66365A23a5978F8BF9100",
    "asset": "ETC",
    "confirmations": 1,
    "amount": 9.9999962
}

http://blockskip:3040/free/send

Request
{
	"asset":"bch",
	"amount":"0.001",
	"to":"1NNAqxsCuBjok78KatfXFAhGauVNgrFWRG",
	"from": "1AkLN1bqvpsqLMArxd8QLAA2qEpVzKY2Qq",
	"privateKey": "U2FsdGVkX19hSGC4cJeq909Gb/L/YhqeV"
}

Response
{
    "asset": "BCH",
    "amount": "0.001",
    "to": "1NNAqxsCuBjok78KatfXFAhGauVNgrFWRG",
    "from": "1AkLN1bqvpsqLMArxd8QLAA2qEpVzKY2Qq",
    "transaction": "39e2189e6469f5a91a385b347e3f68f2e111a9726fab54816984413befd50c04"
}

