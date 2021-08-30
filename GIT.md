git init
git config --global user.name ""
git config --global user.email ""

git config --list

//使用git add添加要提交的文件的时候，如果文件名是中文，会显示数字乱码，使用如下命令进行调整
git config --global core.quotepath false

ssh-keygen
cd ~/.ssh
cat id_rsa.pub