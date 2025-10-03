# \SchemaAPI

All URIs are relative to *http://localhost:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**SchemaPublicRetrieve**](SchemaAPI.md#SchemaPublicRetrieve) | **Get** /v1/schema/public/ | 



## SchemaPublicRetrieve

> map[string]interface{} SchemaPublicRetrieve(ctx).Format(format).Lang(lang).Execute()





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
	format := "format_example" // string |  (optional)
	lang := "lang_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SchemaAPI.SchemaPublicRetrieve(context.Background()).Format(format).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SchemaAPI.SchemaPublicRetrieve``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SchemaPublicRetrieve`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `SchemaAPI.SchemaPublicRetrieve`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSchemaPublicRetrieveRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **format** | **string** |  | 
 **lang** | **string** |  | 

### Return type

**map[string]interface{}**

### Authorization

[tokenAuth](../README.md#tokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/vnd.oai.openapi, application/yaml, application/vnd.oai.openapi+json, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

