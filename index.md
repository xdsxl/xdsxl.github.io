### 用例名称	Import code
### 用例说明	仓库管理员可以从另一个存储库导入代码，可以选择要将代码导入到哪一个存储库，可以变更资料库，需要新建存储库的名称，同时可以选择上市或者私人的。
### 参与者	仓库管理员
### 元素	Import code、change repository、Begin import、understand the supported VCS、Repository name、Privacy、public、private
### 关系	
元素change repository和Begin import对于元素Import code是包含关系；
元素understand the supported VCS是元素Import code的扩展；
元素Repository name和Privacy对于元素change repository是包含关系；
元素Privacy泛化得到元素public和private。
### 建模思路	
仓库管理员可以从另一个存储库Import code，在进行导入代码的时候，如有需要可以进一步understand the supported VCS，可以选择要将代码导入到哪一个存储库，可以change repository，需要新建存储库的名称，Privacy可以选择public，即互联网上的任何人都可以看到此存储库，管理员选择谁可以提交；或者private，即管理员可以选择谁能看到并将文件提交到此存储库。

### 用例名称	Settings
### 用例说明	管理员进入自己创建的仓库中，可以进行设置。包括修改仓库名称，仓库权限的管理，可以启用依赖图、漏洞警报和安全更新，以确保存储库安全和更新。在Webhooks页面，添加当指定的事件发生时，网站将向仓库管理员提供的每个URL发送一个POST请求。可以设置电子邮件地址以在推送事件触发时接收通知，添加部署密钥。设置动作权限和选择保留工件和日志的持续时间，可以设置新的存储库的秘密。
### 参与者	仓库管理员
### 元素
Options、Manage access、Security & analysis、Branches、Webhooks、Deploy keys、Actions、Secrets、Integrations、Who has、 access、Invite a collaborator、Configure security and analysis features、Default branch、Branch protection rules、Add Webhooks、Notifications、Add deploy keys、Actions permissions、Artifact and log retention、Fork pull request workflows、Self-hosted runners、New repository secret、PRIVATE REPOSITORY、DIRECT ACCESS、add another branch.、Upgrade、Address、Approved header、Allow all actions、Disable Actions、Allow local、 actions only、Allow select actions、Add runners、Dependency graph、Dependabot alerts、Dependabot security updates
### 关系
元素Who has access是元素Manage access的扩展；
元素invited any collaborators对于元素Manage access是包含关系；
元素Who has access泛化得到元素PRIVATE REPOSITORY和DIRECT ACCESS；
元素Configure security and analysis features是元素Security & analysis的扩展；
元素Security & analysis泛化得到元素Dependency graph、Dependabot alerts，Dependabot security updates；
元素Add deploy keysDefault branch和Branch protection rules对于Branches是包含关系；
元素add another branch.是元素Default branch的扩展；
元素Upgrade是元素Branch protection rules的扩展；
元素Add Webhooks是Webhooks的扩展；
元素Address和Approved header对于元素Notifications是包含关系；
元素Add deploy keys是Deploy keys的扩展；
元素Actions permissions、Fork pull request workflows、Self-hosted runners对于元素Actions是包含关系；
元素Artifact and log retention是元素Actions的扩展；
元素Actions permissions泛化得到元素Allow all actions、Disable Actions、Allow local actions only、Allow select actions；
元素Add runners是元素Self-hosted runners的扩展；
元素New repository secret是元素Secrets的扩展。
### 建模思路	
管理员进入自己创建的仓库中，可以进行设置。在Options设置页面，可以修改仓库名称，将其设置为模板库，同时可以进行社交预览等。在Manage access设置页面，可以进行仓库权限的管理，即谁有权限访问次仓库，也可以邀请协作者。在Security & analysis页面，可以启用依赖图、漏洞警报和安全更新，以确保存储库安全和更新。在Webhooks页面，添加当指定的事件发生时，网站将向仓库管理员提供的每个URL发送一个POST请求。在Notification页面，设置电子邮件地址以在推送事件触发时接收通知。在Deploy keys页面，可以添加部署密钥。在Actions页面中，可以设置动作权限，包括允许所有动作、禁用动作、仅允许本地操作、允许选择动作，可以选择保留工件和日志的持续时间。在Secrets页面，可以设置新的存储库的秘密，包括此存储库的名称和值。
