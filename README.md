 参数如下：  
|  Name | Value  |
|  --- | --- |
| ENABLE_UNICOM  | 直接填写 true |
| UNICOM_APPID  | 填写获取的 appid |
| UNICOM_USER  | 手机号 |
| UNICOM_PASSWORD  | 服务密码 |    
#### 依次添加共四项

多账号在workflow新建个main1.yml文件，复制之前main.yml全部内容，改一下最后面的，加个数字
  env
user: ${{secrets.unicom_user1}}
                
password: ${{secrets.unicom_password1}}
        
appid: ${{secrets.unicom_appid1}}
最后面那行nodejs不用改
             
 secrets设置密码
| UNICOM_APPID1  | 填写获取的 appid |
| UNICOM_USER1  | 手机号 |
| UNICOM_PASSWORD1  | 服务密码 | 

#### 添加以上数据之后，进入 actions ，点击绿色长条启用它，   

#### 进入日常任务daily-task，然后Enable Workflow启用工作流  


#### 回到代码Code处，进入自述文档README.md,随意编辑它再点击下方绿色Commit changes保存。


#### 并发数我改成2了。
