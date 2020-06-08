husky 是一个 Git Hook 工具，可以在提交前，实现eslint校验和commit校验。

#### 安装依赖
```
// lint-staged 用于实现每次提交只检查本次提交所修改的文件
npm i -D husky lint-staged @commitlint/cli @commitlint/config-conventional
```
> 注意：一定要使用 npm 安装 eslint 和 husky，因为在 windows 操作系统下, 用 yarn 安装依赖，不会触发 husky pre-commit 钩子命令.