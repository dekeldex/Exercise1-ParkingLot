# Exercise1-ParkingLot
Cloud Computing - Exercise 1 - Dekel Binyamin 204845648 | Danielle Guli-Morad 207023029
<br>
<br>
unzip the file
<br>
run the ./setup
<br>
when the setup is finnished the final output will be two endpoints, entry and exit, for example:
<br>
ENDPOINT ENTRY:  https://rphzvo9694.execute-api.us-east-1.amazonaws.com
<br>
ENDPOINT EXIT:  https://uxg8knhf13.execute-api.us-east-1.amazonaws.com
<br>
<br>
you can run entry as such: curl "https://rphzvo9694.execute-api.us-east-1.amazonaws.com/?plate=123-123&parkingLot=387"
<br>
and will get back a ticket id: {"ticketId": "204208e0-b4c9-11eb-99ca-bb21dde0cf03"}
<br>
<br>
take the ticket id and place it in exit: curl "https://uxg8knhf13.execute-api.us-east-1.amazonaws.com/?ticketId=204208e0-b4c9-11eb-99ca-bb21dde0cf03"
<br>
and will get back: {"plate": "123-123", "totalParkedTimeMinuets": 1.8181206186612446, "parkingLot": "387", "price": 0.0}
<br>
<br>
pricing is in 15 minuet increments
