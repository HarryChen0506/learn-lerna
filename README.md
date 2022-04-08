### lerna教程

- 初始化项目

```
$ lerna init
```

- 创建分包

```
$ mkdir core
$ cd core
$ npm init
```

- 为core安装安装外部依赖

```
 $ yarn workspace core add lodash --dev
```

- 为tools安装安装内部依赖

```
# 一定要指定正确的版本号，不然会到npm查找包
$ yarn workspace tools add core@1.0.0
```
