# describeSpecConfig


## 描述
查询缓存Redis实例的规格配置信息

## 请求方式
GET

## 请求地址
https://redis.jdcloud-api.com/v1/regions/{regionId}/specConfig

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**regionId**|String|True| |缓存Redis实例所在区域的Region ID。目前有华北-北京、华南-广州、华东-上海三个区域，Region ID分别为cn-north-1、cn-south-1、cn-east-2|

## 请求参数
无


## 返回参数
|名称|类型|描述|
|---|---|---|
|**result**|[Result](user-content-describespecconfig#result)| |
|**requestId**|String| |

### <div id="result">Result</div>
|名称|类型|描述|
|---|---|---|
|**shardSpec**|Map|单分片规格，自定义分片规格实例才有|
|**instanceSpec**|[InstanceSpec](user-content-describespecconfig#instancespec)|实例规格|
### <div id="instancespec">InstanceSpec</div>
|名称|类型|描述|
|---|---|---|
|**region**|String|region id|
|**instanceVersions**|[VersionInfo[]](user-content-describespecconfig#versioninfo)|版本信息列表|
### <div id="versioninfo">VersionInfo</div>
|名称|类型|描述|
|---|---|---|
|**redisVersion**|String|redis引擎版本：目前支持2.8、4.0|
|**instanceTypes**|[TypeInfo[]](user-content-describespecconfig#typeinfo)|类型信息列表|
### <div id="typeinfo">TypeInfo</div>
|名称|类型|描述|
|---|---|---|
|**instanceType**|String|实例类型：目前支持主从版（master-slave）、集群版（cluster）|
|**specs**|[SpecInfo[]](user-content-describespecconfig#specinfo)|规格列表|
### <div id="specinfo">SpecInfo</div>
|名称|类型|描述|
|---|---|---|
|**memoryGB**|Integer|内存大小（GB）|
|**instanceClass**|String|实例规格，空表示自定义分片集群，只有分片规格，没有实例规格|
|**cpu**|Integer|实例CPU核数，0表示自定义分片集群，CPU核数由分片数变化|
|**diskGB**|Integer|实例磁盘大小（GB)，0表示自定义分片集群，磁盘大小由分片数变化|
|**maxConntion**|Integer|最大连接数，0表示自定义分片集群，最大连接数由分片数变化|
|**bandwidthMbps**|Integer|带宽（Mbps)，0表示自定义分片集群，带宽由分片数变化|
|**ipNumber**|Integer|需要的IP数，0表示自定义分片集群，IP数由分片数变化|
|**shard**|[ShardInfo](user-content-describespecconfig#shardinfo)|该内存对应的分片列表信息，redis 2.8以及redis 4.0主从版没有分片列表信息|
|**azs**|String[]|az列表|
### <div id="shardinfo">ShardInfo</div>
|名称|类型|描述|
|---|---|---|
|**defaultShardNumber**|Integer|默认分片数|
|**defaultShardClass**|String|默认单分片规格代码|
|**shardNumberList**|Integer[]|分片数列表|
|**ipNumberList**|Integer[]|需要的IP数列表|

## 返回码
|返回码|描述|
|---|---|
|**200**|OK|
