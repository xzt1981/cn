# 报警管理

报警管理主要包括报警历史、报警屏蔽两个模块，以实现对报警事件的查询、ACK、屏蔽等操作。

**报警历史**：记录所有发生的报警事件，包括监控对象，报警时间，报警次数、规则、恢复等详情，并允许用户查看报警配置，查图，以及进行ack、手动修复等操作。

- 一次报警事件是一条记录
- 修复：对于无法恢复的报警事件（如更改监控项等配置）进行手动“修复”，不是真正意义的故障修复。
- ACK：记录操作时间和操作人，表示操作人已知报警并将进行修复，对于本次故障事件，将不再发送报警通知。
- 点击操作栏后的“＞”，可查看：报警组、报警次数（已发送报警次数/最大报警次数）、是否屏蔽、报警恢复原因、监控项当前值、NS类型 、监控类别、Tags、报警规则、报警方式等信息

![image](https://github.com/jdcloudcom/cn/blob/DevOps-guhezhu1/image/DevOps/Operation-Guide50.JPG)

**报警屏蔽**：对于有些已知和无需处理的报警事件，可对其设置屏蔽。

屏蔽的报警仍会记录报警历史，只是在屏蔽期间不发送报警通知。

1、按NS屏蔽：屏蔽所选NS的所有报警

2、按规则屏蔽：只屏蔽所选规则的报警，可设置屏蔽某些NS的报警

![image](https://github.com/jdcloudcom/cn/blob/DevOps-guhezhu1/image/DevOps/Operation-Guide51.jpg)
