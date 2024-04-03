# cURL

curl -v -X POST http://localhost:9001/api/promotion -H 'Content-type: application/json' -d '{"promotionCode":"Leo"}'

curl --location 'http://localhost:9001/api/promotion' \
--header 'Content-type: application/json' \
--data '{"promotionCode":"Leo"}'

curl -i -X POST https://reqbin.com/echo/post/json \
     -H 'Content-Type: application/json' \
     -d '{"message":"Hello World!","special_characters":"\/\r\n\t"}'
	 
curl -k https://localhost/my_test_endpoint  : ignore invalid certificat
	 
	 -H 'Content-Type: application/json'