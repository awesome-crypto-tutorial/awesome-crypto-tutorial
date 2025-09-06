# Utterances评论系统设置指南

## 1. 安装Utterances应用

1. 访问 [Utterances应用页面](https://github.com/apps/utterances)
2. 点击 "Install" 按钮
3. 选择 "Install utterances on awesome-crypto-tutorial/awesome-crypto-tutorial.github.io"
4. 点击 "Install" 确认安装

## 2. 配置完成

安装完成后，Utterances会自动工作，无需额外配置！

## 3. 验证设置

1. 构建并部署网站
2. 访问任意一篇文章
3. 在文章底部应该能看到Utterances评论框
4. 尝试发表一条评论测试功能

## 4. 工作原理

- 每篇文章会自动创建一个对应的GitHub Issue
- 评论会显示在该Issue中
- 用户需要GitHub账号才能评论
- 评论数据存储在GitHub Issues中

## 5. 优势

- **完全免费**：基于GitHub Issues，无使用限制
- **安装简单**：只需安装一次应用即可
- **无需配置**：安装后自动工作
- **开源**：代码开源，可自定义
- **快速**：加载速度快

## 6. 注意事项

- 评论者需要有GitHub账号
- 评论数据存储在GitHub Issues中
- 每篇文章会创建一个对应的Issue
- 评论会显示在GitHub仓库的Issues页面

## 7. 自定义设置

在 `_config.yml` 中，你可以调整以下设置：

```yaml
utterances:
  repo: awesome-crypto-tutorial/awesome-crypto-tutorial.github.io  # 你的GitHub仓库
  issue_term: pathname  # 使用路径作为issue标识
  theme: github-light  # 主题
  label: 💬 评论  # issue标签
```

### 主题选项：
- `github-light` - 浅色主题
- `github-dark` - 深色主题
- `github-dark-orange` - 深色橙色主题
- `github-dark-blue` - 深色蓝色主题
- `github-dark-green` - 深色绿色主题
- `github-dark-purple` - 深色紫色主题
- `github-dark-high-contrast` - 深色高对比度主题
- `github-light-high-contrast` - 浅色高对比度主题
- `preferred-color-scheme` - 跟随系统主题

## 8. 故障排除

如果评论框不显示：
1. 确认Utterances应用已安装
2. 确认仓库是公开的
3. 检查网络连接
4. 确认配置正确

## 9. 管理评论

- 评论会显示在GitHub仓库的Issues页面
- 你可以像管理普通Issue一样管理评论
- 可以关闭、删除或编辑评论
- 可以设置Issue模板来自定义评论格式
