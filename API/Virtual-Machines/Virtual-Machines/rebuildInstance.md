# rebuildInstance


## 描述
云主机使用指定镜像重置云主机系统<br>
云主机的状态必须为<b>stopped</b>状态。<br>
若不指定镜像ID，默认使用当前主机的原镜像重置系统。<br>
云主机系统盘类型必须与待更换镜像支持的系统盘类型保持一致，若当前云主机系统盘为local类型，则更换镜像的系统盘类型必须为loaclDisk类型；同理，若当前云主机系统盘为cloud类型，则更换镜像的系统盘类型必须为cloudDisk类型。可查询<a href="http://docs.jdcloud.com/virtual-machines/api/describeimages">DescribeImages</a>接口获得指定地域的镜像信息。<br>
指定的镜像必须能够支持当前主机的实例规格(instanceType)，否则会返回错误。可查询<a href="http://docs.jdcloud.com/virtual-machines/api/describeimageconstraints">DescribeImageConstraints</a>接口获得指定镜像支持的系统盘类型信息。


## 请求方式
POST

## 请求地址
https://vm.jdcloud-api.com/v1/regions/{regionId}/instances/{instanceId}:rebuildInstance

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**regionId**|String|True| |地域ID|
|**instanceId**|String|True| |云主机ID|

## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**password**|String|True| |云主机密码，<a href="http://docs.jdcloud.com/virtual-machines/api/general_parameters">参考公共参数规范</a>。|
|**imageId**|String|False| |镜像ID。可查询<a href="http://docs.jdcloud.com/virtual-machines/api/describeimages">DescribeImages</a>接口获得指定地域的镜像信息。|
|**keyNames**|String[]|False| |密钥对名称；当前只支持一个。仅Linux系统支持指定。|


## 返回参数
无


## 返回码
|返回码|描述|
|---|---|
|**200**|OK|
|**400**|Invalid parameter|
|**401**|Authentication failed|
|**404**|Not found|
|**500**|Internal server error|
|**503**|Service unavailable|
