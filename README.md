# 食用指南

## 安装

```js
git clone https://github.com/Left024/vuepress-theme-vdoing-.git

cd vuepress-theme-vdoing-/

npm install # or yarn install

npm run dev # or yarn dev
```

# 全文搜索

默认的搜索只能搜索一级和二级标题

## 安装

```js
#https://www.npmjs.com/package/vuepress-plugin-fulltext-search
npm i vuepress-plugin-fulltext-search -D
```

## 配置

```js
#docs/.vuepress/config/plugins.js  添加
['fulltext-search'],
```

# Katex

## 安装

```js
#https://vuepress-theme-hope.github.io/md-enhance/zh/
npm i -D vuepress-plugin-md-enhance
```

## 配置

```js
#docs/.vuepress/config/plugins.js  添加
[
      "md-enhance",
      {
        // 启用 TeX 支持
        tex: true,
      },
    ],
```



# 去除首页 banner

个人不喜欢

```js
#执行完 npm install 才会生成文件
#node_modules/vuepress-theme-vdoing/components/Home.vue
#搜索关键字，修改成下面这样
showBanner () { // 当分页不在第一页时隐藏banner栏
        (!this.homeData.postList || this.homeData.postList === 'detailed')
        ? false : true
    },
```

