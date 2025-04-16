# Hexo 博客静态文件

此目录包含由 Hexo 生成的静态网站文件，可直接部署到任何静态网站托管服务。

## 部署说明

这些文件已配置为通过 Cloudflare Workers 使用 Wrangler 部署，但也可以部署到其他平台：

### Cloudflare Workers 部署

1. 确保已安装 [Wrangler CLI](https://developers.cloudflare.com/workers/wrangler/)
2. 运行部署命令：
   ```bash
   wrangler publish
   ```

### 其他部署选项

#### Cloudflare Pages
- 直接连接 GitHub 仓库或上传此 `public` 文件夹

#### Vercel/Netlify
- 拖放此文件夹或连接 Git 仓库

#### 传统主机
- 通过 FTP/SFTP 上传到您的 web 服务器

## 文件结构

```
.
├── index.html        # 首页
├── archives/         # 归档页面
├── categories/       # 分类页面
├── tags/             # 标签页面
├── css/              # 样式表
├── js/               # JavaScript 文件
├── images/           # 图片资源
└── [文章目录]/       # 各文章对应的静态页面
```

## 注意事项

1. 这些是自动生成的静态文件
2. 所有路由已配置为支持干净 URL (无 .html 扩展名)
3. 已预配置 Service Worker 实现 PWA 功能（如主题支持）

## 技术支持

博客使用:
- [Hexo](https://hexo.io/) 静态网站生成器
- [Redefine](https://github.com/EvanNotFound/hexo-theme-redefine) 主题 v2.6.4
- 部署于 Cloudflare 边缘网络

如需帮助，请联系站点管理员。
