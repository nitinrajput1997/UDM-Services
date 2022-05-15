# UDM-Services

![](/udmService.png)

i) Nudm_SubscriberDataManagement
This is used by the network functions to retrieve subscription data from the UDM.

- Nudm_SDM_Get
	this is used by the consumer network functions to retrieve subscriber data

- Nudm_SDM_Notification
	this is used by the UDM to notify network function consumer of update of previous retrieved subscriber data

- Nudm_SDM_Subscriber
	this is used by the network functions (such as AMF, SMF) who subscribe update of UE subscriber data

- Nudm_SDM_Unsubscribe
	this is used by the network function example AMF and SMF to unsubscribe to further notification

- Nudm_SDM_Info
	this is used by the AMF to provide UDM with status information regarding subscription data management procedures toward the UE

ii) Nudm_UEContextManagement
This is used to manage the registration of serving network function with you UDM

- Nudm_UECM_Registration
	This is used to register at udm as the network function serving the UE

- Nudm_UECM_Deregistration
	this is used by the previously register network functions such as AMF SMF to deregister from the UDM

- Nudm_UECM_DeregistrationNotification
	this is used by the udm to notify an AMF said it has been deregistered as serving network function for a UE

- Nudm_UECM_Get
	this is used by the network function to retrieve registration information from udm

- Nudm_UECM_Update
	this is used by the registered network function to update the stored registration information

iii) Nudm_UEAuthentication
This is used by the AUSF to get authentication and provide you UDM with the result of the authentication procedure success

- Nudm_UEAuthentication_Get
	this is used by the AUSF to retrieve authentication data from udm

- Nudm_UEAuthentication_ResultConfirmation
	this is used by the AUSF to inform about the result of an authentication procedure with a UE

iv) Nudm_EventExposure
It allows the network exposure function to subscribe, unsubscribe and get notified about the events from the UDM

- Nudm_EE_Subscribe
	this allows the network function to subscribe or to update event subscription

- Nudm_EE_Unsubscribe
	this allows the network exposure function to delete the subscription to event in UDM that is previously subscribed to

- Nudm_EE_Notify
	this is used by the UDm to report on events that was previously subscribed by the network exposure function

v) Nudm_ParameterProvision
this allows the network function or rather application function via network exposure function for provisioning of an information. Example: expected UE behavior, network configuration parameters.
