# AI-Hunter - API Documentation

## Beacons Page


### MinMax Times
| Data 										|					Description						 									|
| :--- 										| 				:--- 																		|
| **Path:**								|					/{dataset}/conn/minmax 									|
| **Request Params**			|					NA 																			|
| **Type**								|					GET 																		|
| **Response**						|					Minimum(int64),Maximum(int64) 					|
| **Sample Request**      |``curl -s -k -H "Content-Type: application/json" -H "Authorization: Bearer {jwt_token}" https://127.0.0.1/api/v0/mongo/conn/minmax``       							 					 |
| **Sample Output**       | ``{"Minimum":1442285167,"Maximum":1442440793}`` |

### Intervals
| Data 										|							Description						 													|
| :--- 										| 						:--- 																						|
| **Path:**	              |							/{dataset}/beacons/intervals/{beacon_id} 				|
| **Request Params**	    |							beacon_id 															 				|
| **Type**						    |							GET 																		 				|
| **Response**				    |							Array({interval,count}) 								 				|
| **Sample Request**      | ``curl -s -k -H "Content-Type: application/json" -H "Authorization: Bearer {jwt_token}" https://127.0.0.1/api/v0/mongo/beacons/intervals/598e1b080d8b553c838489f3``|
| **Sample Output:**  		| ``[{"interval":1,"count":49},{"interval":2,"count":169},{"interval":3,"count":286}]`` |
