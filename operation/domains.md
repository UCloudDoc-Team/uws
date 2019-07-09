{{indexmenu_n>2}}

# 2、域名管理

创建域名及查看域名的验证状态。

## 创建域名

进入系统后点击“域名管理”页签，先创建需要扫描漏洞的域名。

![](/images/创建域名.png)

选择http或者https，并填写站点域名，点击【验证站长权限】后，将会生成域名对应的验证代码。

**验证方式**

\* 代码验证：请在您的网站首页的header标签里面加上如上代码。例如：

添加的域名www.ucloud.cn的首页为index.html，则在index.html文件中的header标签内添加生成的代码。

''\<header\> ……

\<meta name="ucloud-site-verify"
content="6f93dacb7bae03d4ea95e5d6b45d0dc8" /\> \</header\>''

\* 文件验证：

1.下载专有的HTML验证文件

2.将该文件上传至:您填写的域名服务器上。注意文件名称不要修改,文件名称为:uwebscan\_ucloud.html

3.用浏览器访问http|https://您填写的域名/uwebscan\_ucloud.html,确认是否上传成功

4.点击下面的开始验证

<wrap em>提示:为保持已验证的状态,请验证成功后,也不要删除该html文件。</wrap>

## 查看域名

![](/images/operation/查看域名.png)

<table>
<thead>
<tr class="header">
<th>标题</th>
<th>示例</th>
<th>说明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>站点（域名）</td>
<td><a href="http://www.ucloud.cn">http://www.ucloud.cn</a></td>
<td>用户创建域名是自己选择和填写的域名</td>
</tr>
<tr class="even">
<td>验证状态</td>
<td>验证通过<br />
验证失败</td>
<td>根据验证的结果显示验证状态</td>
</tr>
<tr class="odd">
<td>操作</td>
<td>验证通过——【删除】<br />
验证失败——【验证域名】、【删除】</td>
<td>根据验证状态显示可操作的按钮</td>
</tr>
</tbody>
</table>

## 删除域名

允许删除域名，确认后即删除。如果还需要扫描域名的漏洞，则需要重新创建域名。
