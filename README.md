## Build an Image ##

```docker build --tag <<tagname>> .```


## Run an image ##

```docker run --name <<name>> -p 8090:8080 <<tagname>>```

## Run the curl command ##

This transfers ETH:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"<<dest address>>", "amount":"0.05"}' http://localhost:8090/eth```

This transfers token:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"<<dest address>>"}' http://localhost:8090/token```

