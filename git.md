# 配置身份
```
git config --global user.name "YufeiJiang-gtb"
git config --global user.email "1625229678@qq.com"
```
# 核心工作流
## 初始化仓库
```
cd <项目目录>
git init
```
## 查看当前状态
```
git status
```
红色表示未追踪/已修改，绿色表示已暂存
## 把文件加入暂存区
```
git add .              # 添加所有改动
git add script.py      # 只添加某个文件
```
## 提交（写实验记录）
```
git commit -m "完成 PubMed 搜索工具"
```
## 查看历史
```
git log --oneline      # 简洁版
git log                # 详细版
```
# 连接Github
## 第 1 步：在 GitHub 上新建一个空仓库（不要勾选 README）
## 第 2 步：关联远程仓库
```
# 1. 生成 SSH key（如果还没有）
ssh-keygen -t ed25519 -C "你的邮箱"
# 2. 查看公钥
cat ~/.ssh/id_ed25519.pub
git remote set-url origin git@github.com:YufeiJiang-gtb/agent.git
```
## 第 3 步：推送代码
```
git branch -M main
git push -u origin main
```
