## 常见问题FAQ

Q:如果希望只能通过堡垒机登录主机进行运维，不允许以其他方式登录应如何配置？</br>

A:您可以通过设置该云主机实例的安全组，入/出站规则中只允许堡垒机系统的IP访问该云主机实例；</br>
  或者将所有登录凭据收回，仅在堡垒机系统中保存登录凭据，实现用户只能通过堡垒机系统登录主机。</br>


Q:堡垒机实例里，主机连通性测试失败怎么办？</br>

A:通过以下方式进行排查：</br>
  检查目标主机的相关安全组规则设置是否正确，确保堡垒机实例可以连通主机的相关运维端口。</br>
  检查主机自身防火墙或其它中间设备是否存在其它访问连接限制，例如iptables等。</br>