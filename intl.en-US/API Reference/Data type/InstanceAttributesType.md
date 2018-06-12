# InstanceAttributesType {#InstanceAttributesType .reference}

Lists the ECS instance attributes.

## Node {#section_nhx_2kp_ydb .section}

Depends on the interface.

## Subnodes {#ResponseParameter .section}

|Name |Type |Description |
|:----|:----|:-----------|
|InstanceId |String|Instance ID.|
|InstanceName |String |Instance name.|
|Description|String |Instance description.|
|ImageId |String |ID of the image that is running in the instance.|
|RegionId |String |ID of the region where the instance belongs.|
|ZoneId |String |ID of the zone to which the instance belongs.|
|Cpu |Integer|Number of vCPU.|
|Memory |Integer |Memory size in MB.|
|InstanceType|String |Instance type.|
|InstanceTypeFamily |String |Instance type family.|
|HostName|String |Host name of the instance.|
|SerialNumber|String |Instance serial number.|
|Status |String |Instance status.|
|SecurityGroupIds|[SecurityGroupIdSetType](intl.en-US/API Reference/Data type/SecurityGroupIdSetType.md#)|Security groups that manage the specified instance.|
|PublicIpAddress|[IpAddressSetType](intl.en-US/API Reference/Data type/IpAddressSetType.md#)|Public IP address of the instance.|
|InternetMaxBandwidthIn|Integer |Maximum incoming bandwidth from the public network.|
|InternetMaxBandwidthOut|Integer |Maximum outgoing bandwidth to the public network.|
|InternetChargeType|String |Internet charge type. Possible value:-   PayByTraffic: Billing based on the traffic.

|
|CreationTime|String |Time of creation in the YYYY-MM-DDThh:mm:ssZ format. The value is represented according to [ISO8601](intl.en-US/API Reference/Appendix/ISO 8601 time format.md#),  and  UTC time is used.|
|InstanceNetworkType|String |Network type of the instance. Possible values:-   Classic
-   Vpc

|
|VpcAttributes  |[VpcAttributesType](intl.en-US/API Reference/Data type/VpcAttributesType.md#)|VPC related attributes of an ECS instance.|
|EipAddress|[EipAddressAssociateType](intl.en-US/API Reference/Data type/EipAddressAssociateType.md#)|EIP binding information.|
|InnerIpAddress|[IpAddressSetType](intl.en-US/API Reference/Data type/IpAddressSetType.md#)|Intranet IP address.|
|OperationLocks|[OperationLocksType](intl.en-US/API Reference/Data type/OperationLocksType.md#)|Reason why an instance is locked.|
|InstanceChargeType|String |Instance billing method. Possible values: -   PrePaid: Subscription
-   PostPaid: Pay-As-You-Go

|
|SpottedStrategy|String |The spot strategy of a spot instance.  Possible values:-   NoSpot: A normal Pay-As-You-Go instance. 
-   SpotWithPriceLimit: A price threshold for a spot instance.
-   SpotAsPriceGo: A price that is based on the highest Pay-As-You-Go instance.

Default: NoSpot.|
|DeviceAvailable|Boolean |Whether a new disk can attach to the instance or not.|
|StoppedMode|String |Whether a VPC-Connected ECS instance is charged after it is stopped or not. Possible values:-   KeepCharging: You are billed after the ECS instance is stopped, and its resource and Internet IP address are reserved.
-   StopCharging: You are not billed after the ECS instance is stopped, and its resource  and Internet IP address are not reserved.  You may be unable to restart the instance.
-   Not-applicable: The instance is not applicable for using the StoppedMode parameter.

|
|DeploymentSetId |String |Deployment set ID.|
|NetworkInterfaces |[NetworkInterfaceType ](intl.en-US/API Reference/Data type/NetworkInterfaceType.md#)|The ENI related information.|
|IoOptimized |Boolean |Whether an instance is I/O optimized or not.|
|ExpiredTime |String |Time of expiration in the YYYY-MM-DDThh:mm:ssZ format. The value is represented according to [ISO8601](intl.en-US/API Reference/Appendix/ISO 8601 time format.md#) and  UTC time is used.|
|KeyPairName|String |SSH key pair name.|
