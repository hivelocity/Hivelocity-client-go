# \ContactApi

All URIs are relative to *https://localhost/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteIdResource**](ContactApi.md#DeleteIdResource) | **Delete** /contact/{contactId} | Delete a Contact
[**GetContactResource**](ContactApi.md#GetContactResource) | **Get** /contact/ | Return a list with all Contacts
[**GetIdResource**](ContactApi.md#GetIdResource) | **Get** /contact/{contactId} | Return details of a specific Contact
[**PostContactResource**](ContactApi.md#PostContactResource) | **Post** /contact/ | Create a new Contact
[**PostPasswordReset**](ContactApi.md#PostPasswordReset) | **Post** /contact/password | Recieve a request to reset password, and send a link by email with token
[**PutIdResource**](ContactApi.md#PutIdResource) | **Put** /contact/{contactId} | Edit a Contact
[**PutPasswordReset**](ContactApi.md#PutPasswordReset) | **Put** /contact/password | Recieve a token and password, verify the user and reset your password
[**PutPasswordResource**](ContactApi.md#PutPasswordResource) | **Put** /contact/{contactId}/password | Change password for a Contact


# **DeleteIdResource**
> DeleteIdResource(ctx, contactId)
Delete a Contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **contactId** | **int32**| ID of Contact to View / Update | 

### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetContactResource**
> GetContactResource(ctx, )
Return a list with all Contacts

### Required Parameters
This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetIdResource**
> GetIdResource(ctx, contactId)
Return details of a specific Contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **contactId** | **int32**| ID of Contact to View / Update | 

### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PostContactResource**
> PostContactResource(ctx, payload)
Create a new Contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **payload** | [**ContactLoad**](ContactLoad.md)|  | 

### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PostPasswordReset**
> PostPasswordReset(ctx, payload)
Recieve a request to reset password, and send a link by email with token

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **payload** | [**PasswordRequest**](PasswordRequest.md)|  | 

### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PutIdResource**
> PutIdResource(ctx, contactId, payload)
Edit a Contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **contactId** | **int32**| ID of Contact to View / Update | 
  **payload** | [**ContactUpdate**](ContactUpdate.md)|  | 

### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PutPasswordReset**
> PutPasswordReset(ctx, payload)
Recieve a token and password, verify the user and reset your password

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **payload** | [**PasswordResponse**](PasswordResponse.md)|  | 

### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PutPasswordResource**
> PutPasswordResource(ctx, contactId, payload)
Change password for a Contact

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **contactId** | **int32**| \&quot;ID of Contact to change password\&quot; | 
  **payload** | [**Password**](Password.md)|  | 

### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
