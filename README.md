SmartSSO
========

基于单点登录理念设计的统一多系统用户权限授权中心。

SmartSSO源码需要改的地方
1、SmartSSO global<%@ Application Codebehind="Global.asax.cs" Inherits="WY.SSO.MvcApplication" Language="C#" %>
2、Unity 配置
<container name="defaultContainer">
<register type="SmartSSO.Services.IManageService, SmartSSO" mapTo="SmartSSO.Services.Impl.ManageService, SmartSSO" />
<register type="SmartSSO.Services.IUserManageService, SmartSSO" mapTo="SmartSSO.Services.Impl.UserManageService, SmartSSO" />
<register type="SmartSSO.Services.IProfileService, SmartSSO" mapTo="SmartSSO.Services.Impl.ProfileService, SmartSSO" />
</container>
3、连接字符串
password

