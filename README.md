# Card-Tab 书签卡片式管理，进入管理模式可以自由移动书签位置，添加和删除书签，支持自定义网站分类，支持切换黑暗色主题

#### 2024.09.09 更新：
#### 1、增加私密书签，登录后可见
#### 2、增加网站分类管理，现在你无需编辑代码，通过页面即可进行网站分类的添加和删除操作
#### 3、增加搜索框和一言接口

### 注意：如果你已经部署过前版导航，更新workes代码后将无法看到之前保存的书签，需重新添加书签，望知悉！

#### 2024.09.02 发布 （第一版代码保留在worker-js文件）

#### 演示站点：  https://demo.usgk.us.kg   备用网址：https://demo.linuxdo.nyc.mn   密码：admin

#### 未登录界面
![image](https://github.com/user-attachments/assets/dd0cad75-11ce-4691-804f-b4dff5ae2cde)

#### 已登录界面（黑暗主题）
![image](https://github.com/user-attachments/assets/c18f0df4-8e00-45e6-84db-30f81b545d15)

#### 设置界面
![image](https://github.com/user-attachments/assets/dc91458a-840c-41f9-9e50-261471320f81)



# 部署方法：
#### 五步即可完成部署：
#### 1. 登录 Cloudflare：  https://www.cloudflare.com  创建workers，复制update-workers的代码，然后部署
![image](https://github.com/user-attachments/assets/c067105b-91ee-43d5-90a9-806e5de5fe16)

#### 2. 新建一个名为KV存储
![image](https://github.com/user-attachments/assets/706a7735-b47a-4f66-bdb4-827c38be692b)

#### 3. 添加环境变量，用于设置后台管理密码。变量名为ADMIN_PASSWORD，值your_password换成你自己的密码
![image](https://github.com/user-attachments/assets/532dcb8f-dc30-4ca9-aac9-21ef546bf367)

#### 4. 将workers的CARD_ORDER变量与新建的KV存储绑定，用于存储书签
![image](https://github.com/user-attachments/assets/9b166809-5b1e-451e-be99-253f6e60be54)

#### 5. 添加域名
![image](https://github.com/user-attachments/assets/4f23eab6-e94c-49b1-9198-3c8e05dffa8a)

## 此项目是本人GitHub处女作，各位随意自行魔改，喜欢的话点一下小星星就行，谢谢！
