# Go API client for client

Interact with Hivelocity

## Overview
This API client was generated by the [OpenAPI Generator](https://openapi-generator.tech) project.  By using the [OpenAPI-spec](https://www.openapis.org/) from a remote server, you can easily generate an API client.

- API version: 2.0
- Package version: 1.0.0
- Build package: org.openapitools.codegen.languages.GoClientCodegen

## Installation

Install the following dependencies:

```shell
go get github.com/stretchr/testify/assert
go get golang.org/x/oauth2
go get golang.org/x/net/context
go get github.com/antihax/optional
```

Put the package under your project folder and add the following in import:

```golang
import "./client"
```

## Documentation for API Endpoints

All URIs are relative to *http://localhost/api/v2*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*BandwidthApi* | [**PostDeviceIdBandwidthImageResource**](docs/BandwidthApi.md#postdeviceidbandwidthimageresource) | **Post** /bandwidth/device/{deviceId}/image | Returns RRDTool Graph based bandwidth in PNG format
*BandwidthApi* | [**PostDeviceIdBandwidthResource**](docs/BandwidthApi.md#postdeviceidbandwidthresource) | **Post** /bandwidth/device/{deviceId} | Returns RRDTool Xport based bandwidth data in JSON format
*BandwidthApi* | [**PostServiceIdBandwidthImageResource**](docs/BandwidthApi.md#postserviceidbandwidthimageresource) | **Post** /bandwidth/service/{serviceId}/image | Returns RRDTool Graph based bandwidth in PNG format
*BandwidthApi* | [**PostServiceIdBandwidthResource**](docs/BandwidthApi.md#postserviceidbandwidthresource) | **Post** /bandwidth/service/{serviceId} | Returns RRDTool Xport based bandwidth data in JSON format
*BillingInfoApi* | [**GetBillingInfoResource**](docs/BillingInfoApi.md#getbillinginforesource) | **Get** /billing-info/ | Return a list with all Billing Info
*CancellationApi* | [**GetCancellationDeviceResource**](docs/CancellationApi.md#getcancellationdeviceresource) | **Get** /cancellation/device/{deviceId} | Return the Cancellation found for a Device
*CancellationApi* | [**GetCancellationIdResource**](docs/CancellationApi.md#getcancellationidresource) | **Get** /cancellation/cancellation/{cancellationId} | Return any cancellation by ID
*CancellationApi* | [**GetCancellationResource**](docs/CancellationApi.md#getcancellationresource) | **Get** /cancellation/cancellation | Returns the services cancellations of a client
*CancellationApi* | [**GetCancellationServiceResource**](docs/CancellationApi.md#getcancellationserviceresource) | **Get** /cancellation/service/{serviceId} | Return the Cancellation found for a Service
*CancellationApi* | [**PostCancellationResource**](docs/CancellationApi.md#postcancellationresource) | **Post** /cancellation/cancellation | Creates Cancellation for a device/service
*ContactApi* | [**DeleteContactIdResource**](docs/ContactApi.md#deletecontactidresource) | **Delete** /contact/{contactId} | Delete a Contact
*ContactApi* | [**GetContactIdResource**](docs/ContactApi.md#getcontactidresource) | **Get** /contact/{contactId} | Return details of a specific Contact
*ContactApi* | [**GetContactResource**](docs/ContactApi.md#getcontactresource) | **Get** /contact/ | Return a list with all Contacts
*ContactApi* | [**PostContactResource**](docs/ContactApi.md#postcontactresource) | **Post** /contact/ | Create a new Contact
*ContactApi* | [**PostPasswordReset**](docs/ContactApi.md#postpasswordreset) | **Post** /contact/password | Recieve a request to reset password, and send a link by email with token
*ContactApi* | [**PutContactIdResource**](docs/ContactApi.md#putcontactidresource) | **Put** /contact/{contactId} | Edit a Contact
*ContactApi* | [**PutPasswordReset**](docs/ContactApi.md#putpasswordreset) | **Put** /contact/password | Recieve a token and password, verify the user and reset your password
*ContactApi* | [**PutPasswordResource**](docs/ContactApi.md#putpasswordresource) | **Put** /contact/{contactId}/password | Change password for a Contact
*CreditApi* | [**GetCreditResource**](docs/CreditApi.md#getcreditresource) | **Get** /credit/ | Return a list with all Credits
*CreditApi* | [**GetTotalActiveCreditResource**](docs/CreditApi.md#gettotalactivecreditresource) | **Get** /credit/total | Return the client&#39;s total active credit amount
*CreditApi* | [**PostCreditResource**](docs/CreditApi.md#postcreditresource) | **Post** /credit/ | Receive billing method id and amount and return the created Credit
*DeploymentApi* | [**DeleteDeploymentIdResource**](docs/DeploymentApi.md#deletedeploymentidresource) | **Delete** /deploy/{deploymentId} | Delete the specified deployment
*DeploymentApi* | [**GetDeploymentIdResource**](docs/DeploymentApi.md#getdeploymentidresource) | **Get** /deploy/{deploymentId} | Return a dictionary with deployment information
*DeploymentApi* | [**GetDeploymentResource**](docs/DeploymentApi.md#getdeploymentresource) | **Get** /deploy/ | Return a list with all client deployments
*DeploymentApi* | [**PostDeploymentIdResource**](docs/DeploymentApi.md#postdeploymentidresource) | **Post** /deploy/{deploymentId} | Input a billing info id to process and finish a deployment
*DeploymentApi* | [**PostDeploymentResource**](docs/DeploymentApi.md#postdeploymentresource) | **Post** /deploy/ | Start a new deployment
*DeploymentApi* | [**PutDeploymentIdResource**](docs/DeploymentApi.md#putdeploymentidresource) | **Put** /deploy/{deploymentId} | Receive product, quantity and options to be added on the deployment
*DeviceApi* | [**GetAllDeviceTagOrderResource**](docs/DeviceApi.md#getalldevicetagorderresource) | **Get** /device/tags-order/all | Get all device tags order
*DeviceApi* | [**GetClientDeviceTagOrderResource**](docs/DeviceApi.md#getclientdevicetagorderresource) | **Get** /device/tags-order | Get device tags order for current user
*DeviceApi* | [**GetClientDeviceTagResource**](docs/DeviceApi.md#getclientdevicetagresource) | **Get** /device/tags | Get all device tags for current client
*DeviceApi* | [**GetDeviceIdEventResource**](docs/DeviceApi.md#getdeviceideventresource) | **Get** /device/{deviceId}/events | Returns all Events found for a single device
*DeviceApi* | [**GetDeviceIdResource**](docs/DeviceApi.md#getdeviceidresource) | **Get** /device/{deviceId} | Returns detailed information for a Single Device
*DeviceApi* | [**GetDeviceIpmiWhitelistActionResource**](docs/DeviceApi.md#getdeviceipmiwhitelistactionresource) | **Get** /device/{deviceId}/ipmi/whitelist/{actionId} | Retrieve the state of the action to add the IP into Whitelist
*DeviceApi* | [**GetDeviceIpmiWhitelistPublicIp**](docs/DeviceApi.md#getdeviceipmiwhitelistpublicip) | **Get** /device/{deviceId}/ipmi/whitelist/{actionId}/public-ip | Retrieve the Public IP using the Device ID and the Action ID that was used to add it to Whitelist
*DeviceApi* | [**GetDeviceResource**](docs/DeviceApi.md#getdeviceresource) | **Get** /device/ | Returns Active Devices and basic MetaData
*DeviceApi* | [**GetDeviceTagIdResource**](docs/DeviceApi.md#getdevicetagidresource) | **Get** /device/{deviceId}/tags | Get device tags
*DeviceApi* | [**GetInitialPasswordIdResource**](docs/DeviceApi.md#getinitialpasswordidresource) | **Get** /device/{deviceId}/initial-password | Returns initial password for the device
*DeviceApi* | [**GetIpmiInfoIdResource**](docs/DeviceApi.md#getipmiinfoidresource) | **Get** /device/{deviceId}/ipmi | Returns IPMI info data
*DeviceApi* | [**GetIpmiThresholdsIdResource**](docs/DeviceApi.md#getipmithresholdsidresource) | **Get** /device/{deviceId}/ipmi/thresholds | Returns IPMI thresholds data
*DeviceApi* | [**GetIpmiValidLoginIdResource**](docs/DeviceApi.md#getipmivalidloginidresource) | **Get** /device/{deviceId}/ipmi/valid-login | Returns if device have valid credentials for IPMI login
*DeviceApi* | [**GetNetworkInterfaceResource**](docs/DeviceApi.md#getnetworkinterfaceresource) | **Get** /device/{deviceId}/interfaces | Returns a list of all Network Interfaces bound to a Device
*DeviceApi* | [**GetPowerResource**](docs/DeviceApi.md#getpowerresource) | **Get** /device/{deviceId}/power | Get device&#39;s current power status
*DeviceApi* | [**PostDeviceIpmiWhitelistResource**](docs/DeviceApi.md#postdeviceipmiwhitelistresource) | **Post** /device/{deviceId}/ipmi/whitelist/ | Include the custip (custom IP) on IPMI WhiteList
*DeviceApi* | [**PostPowerResource**](docs/DeviceApi.md#postpowerresource) | **Post** /device/{deviceId}/power | Apply action to device power
*DeviceApi* | [**PutClientDeviceTagOrderResource**](docs/DeviceApi.md#putclientdevicetagorderresource) | **Put** /device/tags-order | Update device tags order for current user
*DeviceApi* | [**PutDeviceIdResource**](docs/DeviceApi.md#putdeviceidresource) | **Put** /device/{deviceId} | Updates Device MetaData for a Single Device
*DeviceApi* | [**PutDeviceTagIdResource**](docs/DeviceApi.md#putdevicetagidresource) | **Put** /device/{deviceId}/tags | Update device tags
*DeviceApi* | [**PutIpmiDevicesThresholdsIdResource**](docs/DeviceApi.md#putipmidevicesthresholdsidresource) | **Put** /device/ipmi/thresholds | Updates IPMI thresholds for device list
*DeviceApi* | [**PutIpmiThresholdsIdResource**](docs/DeviceApi.md#putipmithresholdsidresource) | **Put** /device/{deviceId}/ipmi/thresholds | Updates IPMI thresholds data
*InventoryApi* | [**GetStockByProductResource**](docs/InventoryApi.md#getstockbyproductresource) | **Get** /inventory/product/{productId} | Return a structured sps stock data, grouped by city or facility code for a single product
*InventoryApi* | [**GetStockResource**](docs/InventoryApi.md#getstockresource) | **Get** /inventory/product | Return a structured sps stock data, grouped by city or facility code for all products
*InvoiceApi* | [**GetInvoiceIdDetails**](docs/InvoiceApi.md#getinvoiceiddetails) | **Get** /invoice/{invoiceId}/details | Return detailed information for an invoice
*InvoiceApi* | [**GetInvoiceIdResource**](docs/InvoiceApi.md#getinvoiceidresource) | **Get** /invoice/{invoiceId} | Return serialized data on a single invoice
*InvoiceApi* | [**GetInvoicePdfResource**](docs/InvoiceApi.md#getinvoicepdfresource) | **Get** /invoice/{invoiceId}/pdf-download | Return an Invoice PDF file in Base64 Encoded Format
*InvoiceApi* | [**GetInvoiceResource**](docs/InvoiceApi.md#getinvoiceresource) | **Get** /invoice/ | Return serialized data on all invoices
*OrderApi* | [**GetOrderIdResource**](docs/OrderApi.md#getorderidresource) | **Get** /order/{orderId} | Return details of a specific Order
*OrderApi* | [**GetOrderResource**](docs/OrderApi.md#getorderresource) | **Get** /order/ | Return a list with all Orders
*PermissionApi* | [**GetPermissionAllResource**](docs/PermissionApi.md#getpermissionallresource) | **Get** /permission/ | Endpoint to get All Permissions
*PermissionApi* | [**GetPermissionContactResource**](docs/PermissionApi.md#getpermissioncontactresource) | **Get** /permission/contact/{contactId} | Endpoint to get Contact Permissions
*PermissionApi* | [**GetPermissionUserResource**](docs/PermissionApi.md#getpermissionuserresource) | **Get** /permission/user | Endpoint to get User Permissions
*PermissionApi* | [**PostPermissionAssignContactResource**](docs/PermissionApi.md#postpermissionassigncontactresource) | **Post** /permission/contact | Endpoint to assign a new Permission to a Contact
*ProductApi* | [**GetProductOperatingSystemsResource**](docs/ProductApi.md#getproductoperatingsystemsresource) | **Get** /product/{productId}/operating-systems | Return List of operating systems found for a Product
*ProductApi* | [**GetProductOptionResource**](docs/ProductApi.md#getproductoptionresource) | **Get** /product/{productId}/options | Return List of Options found for a Product
*ProductApi* | [**PostProductMatchResource**](docs/ProductApi.md#postproductmatchresource) | **Post** /product/match | Return a list of Products matching the provided lshw output of a server
*ProfileApi* | [**GetBasicProfileResource**](docs/ProfileApi.md#getbasicprofileresource) | **Get** /profile/basic | Get Basic Profile of current user or a contact with id
*ProfileApi* | [**GetProfileResource**](docs/ProfileApi.md#getprofileresource) | **Get** /profile/ | Get Profile of current user or a contact with id
*ProfileApi* | [**PutProfileResource**](docs/ProfileApi.md#putprofileresource) | **Put** /profile/ | Update Profile of current user or a contact with id
*ServiceApi* | [**GetServiceIdResource**](docs/ServiceApi.md#getserviceidresource) | **Get** /service/{serviceId} | Return a dictionary with data from a specific account service
*ServiceApi* | [**GetServiceResource**](docs/ServiceApi.md#getserviceresource) | **Get** /service/ | Return a list of all account services
*SshKeyApi* | [**DeleteSshKeyIdResource**](docs/SshKeyApi.md#deletesshkeyidresource) | **Delete** /ssh_key/{sshKeyId} | Removes public ssh key
*SshKeyApi* | [**GetSshKeyResource**](docs/SshKeyApi.md#getsshkeyresource) | **Get** /ssh_key/ | Gets all public ssh key
*SshKeyApi* | [**PostSshKeyResource**](docs/SshKeyApi.md#postsshkeyresource) | **Post** /ssh_key/ | Adds public ssh key
*SshKeyApi* | [**PutSshKeyIdResource**](docs/SshKeyApi.md#putsshkeyidresource) | **Put** /ssh_key/{sshKeyId} | Updates public ssh key
*TicketApi* | [**GetTicketIdResource**](docs/TicketApi.md#getticketidresource) | **Get** /tickets/{ticketId} | Returns details of a specific ticket
*TicketApi* | [**GetTicketReplyResource**](docs/TicketApi.md#getticketreplyresource) | **Get** /tickets/{ticketId}/reply | Returns a reply for a specific ticket
*TicketApi* | [**GetTicketResource**](docs/TicketApi.md#getticketresource) | **Get** /tickets/ | Returns a list with all Tickets
*TicketApi* | [**GetTicketSearchResource**](docs/TicketApi.md#getticketsearchresource) | **Get** /tickets/search | Return results of ticket search
*TicketApi* | [**PostTicketReplyResource**](docs/TicketApi.md#postticketreplyresource) | **Post** /tickets/{ticketId}/reply | Creates reply for a specific Ticket
*TicketApi* | [**PostTicketResource**](docs/TicketApi.md#postticketresource) | **Post** /tickets/ | Creates a new ticket
*TicketApi* | [**PutTicketIdResource**](docs/TicketApi.md#putticketidresource) | **Put** /tickets/{ticketId} | Updates a specific ticket
*TokenApi* | [**DeleteTokenIdResource**](docs/TokenApi.md#deletetokenidresource) | **Delete** /token/{token} | Deletes the Public API Token
*TokenApi* | [**GetTokenIdResource**](docs/TokenApi.md#gettokenidresource) | **Get** /token/{token} | Returns Public API Token
*TokenApi* | [**GetTokenResource**](docs/TokenApi.md#gettokenresource) | **Get** /token/ | Returns a list of Public API Tokens for the current user
*TokenApi* | [**PostTokenResource**](docs/TokenApi.md#posttokenresource) | **Post** /token/ | Create a new Public API Token for the current user
*TokenApi* | [**PutTokenIdResource**](docs/TokenApi.md#puttokenidresource) | **Put** /token/{token} | Updates the Public API Token
*WebhookApi* | [**DeleteWebhookIdResource**](docs/WebhookApi.md#deletewebhookidresource) | **Delete** /webhooks/{webhookId} | Deletes a single webhook
*WebhookApi* | [**GetWebhookEventResource**](docs/WebhookApi.md#getwebhookeventresource) | **Get** /webhooks/events | Returns all available Webhook Events
*WebhookApi* | [**GetWebhookIdResource**](docs/WebhookApi.md#getwebhookidresource) | **Get** /webhooks/{webhookId} | Returns detailed information for a Single Webhook
*WebhookApi* | [**GetWebhookResource**](docs/WebhookApi.md#getwebhookresource) | **Get** /webhooks/ | Returns your active Webhooks
*WebhookApi* | [**PostEventScriptActionTriggerResource**](docs/WebhookApi.md#posteventscriptactiontriggerresource) | **Post** /webhooks/trigger | Queues a webhook for the event script action that was triggered
*WebhookApi* | [**PostWebhookResource**](docs/WebhookApi.md#postwebhookresource) | **Post** /webhooks/ | Create a new Webhook for a Webhook Event
*WebhookApi* | [**PutWebhookIdResource**](docs/WebhookApi.md#putwebhookidresource) | **Put** /webhooks/{webhookId} | Updates a Single Webhook


## Documentation For Models

 - [CancellationCreate](docs/CancellationCreate.md)
 - [ContactCreate](docs/ContactCreate.md)
 - [ContactUpdate](docs/ContactUpdate.md)
 - [CreateCredit](docs/CreateCredit.md)
 - [DeploymentCustomization](docs/DeploymentCustomization.md)
 - [DeploymentStart](docs/DeploymentStart.md)
 - [DeviceInterface](docs/DeviceInterface.md)
 - [DeviceIpmiThresholds](docs/DeviceIpmiThresholds.md)
 - [DeviceIpmiWhitelistIp](docs/DeviceIpmiWhitelistIp.md)
 - [DeviceTag](docs/DeviceTag.md)
 - [DeviceUpdate](docs/DeviceUpdate.md)
 - [OperatingSystem](docs/OperatingSystem.md)
 - [Password](docs/Password.md)
 - [PasswordRequest](docs/PasswordRequest.md)
 - [PasswordResponse](docs/PasswordResponse.md)
 - [Permission](docs/Permission.md)
 - [ProductMatch](docs/ProductMatch.md)
 - [ProductOption](docs/ProductOption.md)
 - [ProfileUpdate](docs/ProfileUpdate.md)
 - [PublicApiTokenLoad](docs/PublicApiTokenLoad.md)
 - [SshKey](docs/SshKey.md)
 - [SshKeyUpdate](docs/SshKeyUpdate.md)
 - [Stock](docs/Stock.md)
 - [TicketCreate](docs/TicketCreate.md)
 - [TicketCreateReply](docs/TicketCreateReply.md)
 - [TicketPut](docs/TicketPut.md)
 - [UpdateDevicesIpmiThresholds](docs/UpdateDevicesIpmiThresholds.md)
 - [WebhookCreate](docs/WebhookCreate.md)
 - [WebhookUpdate](docs/WebhookUpdate.md)


## Documentation For Authorization



## apiKey

- **Type**: API key

Example

```golang
auth := context.WithValue(context.Background(), sw.ContextAPIKey, sw.APIKey{
    Key: "APIKEY",
    Prefix: "Bearer", // Omit if not necessary.
})
r, err := client.Service.Operation(auth, args)
```



## Author



