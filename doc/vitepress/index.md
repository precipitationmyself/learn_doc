---
prev:
  text: '源码'
  link: '../SourceCode/vueuse'
next: '../SourceCode/vueuse'
---

# vitepress使用说明
## 配置说明
```js
export default defineConfig({
  title: "learn_doc",
  description: "A VitePress Site",
  themeConfig: {
    // https://vitepress.dev/reference/default-theme-config
    nav: [
      { text: 'Home', link: '/' },
      { text: 'Examples', link: '/markdown-examples' },
      { text: '源码', link: '/doc/SourceCode/vueuse' },
      { text: 'vitepress', link: '/doc/vitepress/index' },
    ], // 导航栏

    sidebar: {
      "/markdown-examples":[
        {
          text: 'Examples',
          items: [
            { text: 'Markdown Examples', link: '/markdown-examples' },
            { text: 'Runtime API Examples', link: '/api-examples' }
          ]
        }
      ],
      "/doc/SourceCode/vueuse":[
        {
          text: 'vueuse',
          items: [
            { text: 'Markdown Examples', link: '/markdown-examples' },
          ]
        }
      ]
    }, // 侧边栏配置

    socialLinks: [
      { icon: 'github', link: 'https://github.com/precipitationmyself/learn_doc' }
    ] // 右上角社交链接
  }
})
```
## 使用说明
```md
配置上下页
---
prev:
  text: 'Markdown'
  link: '/guide/markdown'
---
```
