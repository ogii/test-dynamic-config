# test-dynamic-config
Testing dynamic configs with both orbs

## Sample API call using curl
Please adjust the project slug when making the API call.

```
curl --location --request POST 'https://circleci.com/api/v2/project/github/ogii/test-dynamic-config/pipeline' \
--header "Circle-Token: $CIRCLECI_TOKEN" \
--header 'Content-Type: application/json' \
--data-raw '{
    "parameters": { 
        "my-pipeline-param-api": true
    }
}'
```
