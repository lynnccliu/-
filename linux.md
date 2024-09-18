# 系统目录结构
/bin 存放常用命令
/boot 启动linux核心文件
/dev 存放linux外部设备
/etc 系统管理所需的配置文件和子目录
/home 用户的主目录
/lib library,共享库，所有应用程序都要用到这些共享库
/opt optional的缩写，给主机额外安装软件所摆放的目录
/proc processes，/proc是一种伪文件系统，访问这个目录来获取系统信息
/root 系统管理员
/sbin superuser binaries,存放系统管理员使用的系统管理程序。
/var variable,存放着在不断扩充的东西，我们习惯将哪些经常被修改的目录放在目录下，包括各种日志文件。
/run 是一个临时文件系统，存储系统启动以来的信息。
# 文件与目录管理
## 路径
### 绝对路径
根目录/开头
### 相对路径
../
## 处理目录命令
ls(list files) 列出目录及文件名 -a:全部文件；-d：仅列出目录本身;-l：长数据串列出，包含文件的属性与权限等等数据；
cd(change directory) 切换目录 [相对路径或绝对路径]
pwd(print work directory) 显示目前的目录 -p：显示出确实的路径
mkdir(make directory) 创建一个新的目录, -m配置文件的权限，-p:递归创建多层目录
rmdir(remove directory) 删除一个空的目录，-p一次删除多级目录
cp(copy file) 复制文件或目录
rm(remove) 删除文件或目录，-f：force,忽略不存在的文件不会出现告警；-i：互动模式，在删除前会询问使用者是否动作；-r:递归删除，最常用在目录的删除了，非常危险操作！！！
mv(move file) 移动文件与目录。-f；-i：若目标文件已经存在时，会询问是否覆盖；-u：若目标文件已经存在，且source比较新，才会update；
**man命令可查看各个命令的使用文档**
## 查看文件内容
cat:由第一行开始显示文件内容
tac：从最后一行开始显示
nl:
