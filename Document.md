## Gitflow使用文档
```bash
// 安装Gitflow
pnpm install -g gitflow

// 初始化Gitflow
git flow init

// 创建功能分支
git flow feature start newFeature（"功能描述"）

// 开发功能
git add .
git commit -m "message"

// 完成功能开发并合并到开发分支
git flow feature finish newFeature

// 创建发布分支
git flow release start 1.0(版本号)

// 发布分支中进行最后的测试修改
git add .
git commit -m "message"

// 完成发布分支并合并到主分支和开发分支，同时打上标签
git flow release finish 1.0

// 创建一个热修复分支
git flow hotfix start 1.0.1(版本号)

// 在热修复分支上进行修补
git add .
git commit -m "message"

// 完成热修复并合并到主分支和开发分支
git flow hotfix finish 1.0.1

// 链接远程仓库
git remote add origin https://github.com/username/repository.git

// 推送 main 和 develop 分支到远程仓库
git push origin main
git push origin develop

// 查看标签
git tag

// 推送标签到远程仓库
git push origin --tags
```