# about how to setting git on mac

第一次用mac 做上传实验

1、下载git
2、control+左键 打开 安装文件
3、打开终端  git --version 检查版本 看是否安装
4、创建一个全局的用户名、全球邮箱
git config --global user.name "shengyao"
git config --global user.email "MY_NAME@example.com"

5、让本地和 github进行关联
    cd ~进入根目录 （笨方法 可以用cd ..进入上一级目录 知道上到根目录）
    <img src="https://github.com/Ljhandnds123/new/blob/master/git.png" width="200" height="200"/> 
    将SSH key添加到GitHub。登录到GitHub页面，Account Settings->SSH Public Keys->Add another key
    将生成的key(id_rsa.pub文件）内容copy到输入框中，save。
    commd+shift+g进入/Users/chen/.ssh/就可以看得见私钥和公钥
    私钥的名字是 id_rsa，是服务器确定你身份的唯一凭证。
    公钥的名字是id_rsa.pub。把这个文件发给仓库管理员，仓库管理员会把这个公钥放到服务器上，以后git就通过上面的私钥跟服务器交互了。如果使用github就是自己把公钥内容添加上去
6、找一个目录执行git clone http://xxx.git（从服务器端克隆git库，当然这个要服务器管理员给你权限和帐号），以后xxx目录就是一个git目录，可以在这个目录下执行git操作






三、 linux基础命令
sudo -s   获取绝对用户权限
cd xxx    进入xxx目录
ls (-a/-A)   显示当前路径下所有文件(隐藏的)
pwd       显示当前绝对路径
mkdir  xxx   创建文件夹xxx
man xxx     查看xxx命令手册

然后介绍下Git基础命令的含义；
clone   克隆远程仓库
init       初始化仓库
remote 连接远程仓库
pull      从远程仓库下拉获取新数据
push    将本地仓库新增或修改文件上传到远程仓库
add     添加文件或者修改文件，commit以及push之前使用
log      当前仓库提交过的日志信息
status  当前仓库版本状态
commit 提交到当前仓库中
branch 分支命令，相关增删查操作
checkout 使用远程仓库最后一个版本完全覆盖当前仓库内容／选择分支branch
diff      对比版本内容
merge   合并版本内容
