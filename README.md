

### git



```sh

echo "# committedTest" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:I-adore-you/committedTest.git
git push -u origin main
```









```sh
git remote add origin git@github.com:I-adore-you/committedTest.git
git branch -M main
git push -u origin main
```







`git 相关命令`







要查看当前的Git全局配置信息，您可以使用以下命令：

```
git config --global --list
```

运行此命令后，将显示您当前的Git全局配置信息，包括用户名、邮箱地址等。

Question :

![img](http://ideapp/assets/icons/edit-icon.png)

怎么配置git 的邮箱和用户名信息， 给出命令

Answer :

![img](http://ideapp/assets/icons/refresh.png)



![Share icon](http://ideapp/assets/images/sharing-icons/share.png)

要配置Git的邮箱和用户名信息，您可以使用以下命令：  设置全局邮箱：

```
git config --global user.email "your_email@example.com"
```

设置全局用户名：

```
git config --global user.name "Your Name"
```

请将 "your_email@example.com" 替换为您的邮箱地址，将 "Your Name" 替换为您的用户名。这些命令将在全局范围内配置Git的邮箱和用户名信息，以便在提交代码时正确标识您的身份。

Question :

![img](http://ideapp/assets/icons/edit-icon.png)

怎么删除git的一些全局配置给出命令

Answer :

![img](http://ideapp/assets/icons/refresh.png)



![Share icon](http://ideapp/assets/images/sharing-icons/share.png)

要删除Git的全局配置，您可以使用以下命令：  删除全局邮箱配置：

```
git config --global --unset user.email
```

删除全局用户名配置：

```
git config --global --unset user.name
```

这些命令将删除全局配置中的对应项，使其恢复为默认值或空值。这样，Git将不再使用全局配置中的邮箱和用户名信息。







### 注意

> **邮箱地址不匹配!**

但是为什么GitHub上面并没有显示贡献（没有绿色的方块展示）

Answer :

如果您在本地进行了代码修改并将其提交到远程仓库，但在GitHub上没有显示贡献（即没有绿色的方块展示），可能有几个原因：

1. 邮箱地址不匹配：GitHub根据提交的邮箱地址来确定贡献者。请确保您在本地Git配置中使用的邮箱地址与您GitHub帐户关联的邮箱地址匹配。  
2. . 分支问题：如果您在一个分支上进行了修改并将其推送到远程仓库，但在默认分支上没有合并或拉取这些更改，那么贡献可能不会显示在默认分支上。 
3. 仓库权限：如果您没有足够的权限来推送更改到远程仓库，那么贡献也不会被记录。  请检查以上问题，并确保您的本地设置和操作都正确，以便在GitHub上正确显示您的贡献。





> GitHub 邮箱 私有问题

我是用git push 提交出现 You can make your email public or disable this protection by visiting:  是为什么

Answer :

![img](http://ideapp/assets/icons/refresh.png)



![Share icon](http://ideapp/assets/images/sharing-icons/share.png)

当您使用 `git push` 命令提交代码时，如果您的邮箱地址是私有的或被GitHub视为敏感信息，GitHub会向您发送一条警告消息，内容类似于："You can make your email public or disable this protection by visiting:"。  这是GitHub的一项安全功能，旨在保护用户的隐私。默认情况下，GitHub会自动隐藏提交者的邮箱地址，以防止恶意用户或机器人获取到这些信息。如果您希望在提交中显示您的邮箱地址，您可以按照警告消息中提供的链接，访问相关设置页面，并选择将您的邮箱地址设为公开。请注意，公开您的邮箱地址可能会增加收到垃圾邮件或其他不必要的联系的风险。因此，在进行此操作之前，请确保您已充分考虑了相关风险和隐私问题。

Question :

![img](http://ideapp/assets/icons/edit-icon.png)

但是这不就矛盾了吗， GitHub 既需要 根据 提交者的邮箱 来表明贡献者， ；配置了邮箱之后，又出现上面情况？

Answer :

![img](http://ideapp/assets/icons/refresh.png)



![Share icon](http://ideapp/assets/images/sharing-icons/share.png)

是的，这确实有些矛盾。GitHub默认情况下会根据提交者的邮箱来标识贡献者，但是在某些情况下，GitHub也会隐藏提交者的邮箱地址，以保护用户的隐私。如果您的邮箱地址被隐藏了，那么在提交中就不会显示您的贡献。但是，即使您的邮箱地址被隐藏了，GitHub仍然会记录您的贡献，只是不会在提交中显示出来。如果您希望在提交中显示您的贡献，您可以按照警告消息中提供的链接，将您的邮箱地址设为公开。但是请注意，公开您的邮箱地址可能会增加收到垃圾邮件或其他不必要的联系的风险。







![image-20230721181010477](../README.assets/image-20230721181010477.png)