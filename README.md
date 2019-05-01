# IosevkaYt

这个是 [Iosevka](https://github.com/be5invis/Iosevka) 中 `cc` 字体的非连体字版的修改方法。

**本工程基于 [Iosevka](https://github.com/be5invis/Iosevka) 2.2.1 测试通过。**

## 修改方法

修改 `parameters.toml` 文件，在该文件里找到以下内容

```
[cc]
inherits = ["xx-cc"]
spacing = 3
```

在这些内容下添加一行内容 `disableLigation = true` ，变成以下内容。

```
[cc]
inherits = ["xx-cc"]
spacing = 3
disableLigation = true
```

## 编译方法

用原来 [Iosevka](https://github.com/be5invis/Iosevka) 的方法编译就行。

```
npm run build -- contents::iosevka-cc
```
