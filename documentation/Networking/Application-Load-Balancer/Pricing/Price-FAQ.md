
# 应用负载均衡计费FAQ

[1.负载均衡实例费如何计算？](Price-FAQ#user-content-1)

[2.负载均衡流量费如何计算？](Price-FAQ#user-content-2)

[3.内网负载均衡是否收取流量费？](Price-FAQ#user-content-3)

[4.公网IP流量费和负载均衡流量费有什么不同？](Price-FAQ#user-content-4)

[5.通过哪种方式可计算负载均衡的流量，从而计算流量费？](Price-FAQ#user-content-5)

[6.健康检查的流量是否会被计费？](Price-FAQ#user-content-6)

## 1.负载均衡实例费如何计算？
<div id="user-content-1"></div>

负载均衡实例费是基础的资源占用费，不管负载均衡实例是否转发业务流量都会固定收取，按照实际使用时长收取，具体价格为5.52元/天(0.23元/小时)

## 2.负载均衡流量费如何计算？
<div id="user-content-2"></div>

流量费是指经由负载均衡处理的用户业务流量产生的费用，依据负载均衡实际处理的出方向和入方向业务流量的总和收费，如负载均衡未转发任何业务流量，将不收取流量费。

## 3.内网负载均衡是否收取流量费？
<div id="user-content-3"></div>

内网负载均衡也收取流量费。无论内网负载均衡还是公网负载均衡，流量作为系统为您分配负载均衡资源规格的一个衡量系数，系统通过您实际使用的流量大小分配不同规格的负载均衡资源，以满足您的业务需求。流量费收取的是不同规格的负载均衡资源费用。

## 4.弹性公网IP流量费和负载均衡流量费有什么不同？
<div id="user-content-4"></div>

如果负载均衡均衡绑定了弹性公网IP，弹性公网IP作为独立的产品单独计费。负载均衡流量费指的是经由负载均衡处理的用户业务流量产生的费用，流量的大小作为系统为您分配负载均衡资源规格的一个衡量系数，系统通过您实际使用的流量大小分配不同规格的负载均衡资源。

## 5.通过哪种方式可计算负载均衡的流量，从而计算流量费？
<div id="user-content-5"></div>

当负载均衡正式收费后，可以通过负载均衡监控项“总字节数”计算流量大小，目前该监控项统计数据存在偏差，不作为计算流量大小的参考标准。

## 6.健康检查的流量是否会被计费？
<div id="user-content-6"></div>

流量费收取的是经由负载均衡处理的用户业务流量产生的费用，负载均衡健康检查的流量不会被计费。

