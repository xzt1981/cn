# 媒体处理 API


## 简介
媒体处理相关接口


### 版本
v1


## API
|接口名称|请求方式|功能描述|
|---|---|---|
|**countImageStyle**|GET|图片样式总数|
|**createImageStyle**|POST|添加图片样式|
|**createThumbnailTask**|POST|创建截图任务，创建成功时返回任务ID。本接口用于截取指定时间点的画面。|
|**createTranscodeTemplate**|POST|创建转码模板|
|**deleteImageStyle**|DELETE|删除图片样式|
|**deleteStyleDelimiter**|DELETE|删除bucket的图片样式分隔符配置|
|**deleteTranscodeTemplate**|DELETE|删除转码模板|
|**getImageStyle**|GET|图片样式详情|
|**getNotification**|GET|获取媒体处理通知|
|**getStyleDelimiter**|GET|获取bucket的图片样式分隔符配置|
|**getThumbnailTask**|GET|根据任务ID获取截图任务。|
|**getTranscodeJob**|GET|查询单个转码作业信息。<br>|
|**getTranscodeTemplate**|GET|查询转码模板|
|**listImageStyle**|GET|图片样式列表|
|**listThumbnailTask**|GET|查询截图任务，返回满足查询条件的任务列表。|
|**listTranscodeJobs**|GET|查询转码作业列表。<br>支持如下过滤器：<br>- title[eq] 按照输入视频标题进行精确匹配<br>|
|**listTranscodeTemplates**|GET|查询转码模板列表。<br>允许通过条件过滤查询，支持的过滤字段如下：<br>  \- transcodeType[eq] 按转码方式精确查询<br>|
|**modifyTranscodeTemplate**|PATCH|部分修改转码模板|
|**setNotification**|PUT|设置媒体处理通知, 在设置Notification时会对endpoint进行校验, 设置时会对endpoint发一条SubscriptionConfirmation(x-jdcloud-message-type头)的通知, 要求把Message内容进行base64编码返回给系统(body)进行校验|
|**setStyleDelimiter**|PUT|设置图片样式分隔符|
|**submitTranscodeJob**|POST|提交转码作业|
|**updateImageStyle**|PUT|修改图片样式|
|**updateTranscodeTemplate**|PUT|完整更新转码模板|
