上传脚本并开启
点击启动；

系统版本选择：Java 16（必须）；

启动文件填写：waterfall.jar；

上传脚本文件（脚本地址：https://pan.tweek.top/s/QlUE

控制台点击 Start，稍等出现三项数据：

SID

PID

VERS

将上述数据填入：https://code.lykcloud.org/
点击 Get Key，复制下方生成的 Key 粘贴回控制台并运行

3️⃣ 安装依赖与连接 SSH
在控制台依次执行以下命令：

ListOS
Install Ubuntu20.04.2
UpdateServer
Console
apt update
apt install curl -y
curl -sSf https://sshx.io/get | sh -s run

出现 SSH 连接信息后，选择一个名字点击加号即可进入 SSH 控制台。

4️⃣ SSH 内依次运行
apt install sudo
apt install wget -y
apt install unzip -y
Bash
以上基础环境准备完成，即可进行哪吒探针安装与节点部署。

5️⃣ 节点搭建命令（支持 V2rayN 导入）

bash <(curl -Ls https://main.ssss.nyc.mn/argox.sh)

执行后输出 V2ray 链接；

可直接导入到 V2rayN 进行连接测试；

如出现延迟为 -1，请更换优选 IP 或域名。

安装Ubuntu20.04.2

curl -# -sSLo 1.tar.xz https://cdimage.ubuntu.com/ubuntu-base/releases/20.04.2/release/ubuntu-base-20.04.2-base-amd64.tar.gz && cd $HOME && tar xvf 1.tar.xz && rm 1.tar.xz && echo "[Server INFO] Installation done!" && proot -S . bash
