# Python Blockchain to help myself to better understand how the technology works


#### If you would like to test this blockchain, you will need [Postman](https://www.getpostman.com/) or you can use cURL.

1. Clone this repo
2. Run the script with [Python 3.6](https://www.python.org/downloads/)
3. Using Postman, make a GET request to http://localhost:5000/mine
  - this will create a new block in the Blockchain
4. You will want to copy the transactions object containing `'amount'`, `'recipient'`, and `'sender'`
5. In Postman, make a POST request to http://localhost:5000/transactions/new
  - You will add the transactions object you copied from your GET response to the body in the POST request
  - You should receive a response that reads some thing like `"message": "Transaction will be added to Block 1"`

###### Additionally, you may run the same script on a different server, say `http://localhost:5001` to see that the blockchain nodes will update from additional servers and keep a history of previous transactions made.
