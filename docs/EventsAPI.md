# \EventsAPI

All URIs are relative to *http://localhost:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**PublishEvent**](EventsAPI.md#PublishEvent) | **Post** /v1/public/events/ | Publish analytics event



## PublishEvent

> EventAcceptedResponse PublishEvent(ctx).PublishEventRequest(publishEventRequest).Execute()

Publish analytics event



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	publishEventRequest := *openapiclient.NewPublishEventRequest("SessionId_example") // PublishEventRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EventsAPI.PublishEvent(context.Background()).PublishEventRequest(publishEventRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EventsAPI.PublishEvent``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PublishEvent`: EventAcceptedResponse
	fmt.Fprintf(os.Stdout, "Response from `EventsAPI.PublishEvent`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPublishEventRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **publishEventRequest** | [**PublishEventRequest**](PublishEventRequest.md) |  | 

### Return type

[**EventAcceptedResponse**](EventAcceptedResponse.md)

### Authorization

[tokenAuth](../README.md#tokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

