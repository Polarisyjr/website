# 访客地图设置指南

## 🗺️ 功能说明

访客地图已集成到您的主页底部，可以显示访客的地理位置分布。您可以选择：

1. **仅后台记录**：不显示地图，但可以查看访客数据
2. **公开显示**：在主页底部显示访客地图

## ⚙️ 配置方法

### 1. 启用/禁用访客地图

在 `_config.yml` 文件中找到以下配置：

```yaml
visitor_map:
  enabled: false # 改为 true 启用，false 禁用
  title: "访客地图" # 地图标题
  description: "感谢来自世界各地的访客！" # 描述文字
  clustrmaps_id: # 您的 ClustrMaps ID
  show_analytics_link: true # 是否显示后台链接
```

### 2. 获取 ClustrMaps ID（推荐）

1. 访问 [ClustrMaps.com](https://clustrmaps.com/)
2. 注册免费账户
3. 添加您的网站
4. 获取地图代码中的 ID
5. 将 ID 填入 `clustrmaps_id` 字段

### 3. 配置选项

- `enabled: true/false` - 是否显示访客地图
- `title` - 地图标题
- `description` - 描述文字
- `clustrmaps_id` - ClustrMaps 的 ID
- `show_analytics_link: true/false` - 是否显示后台链接

## 📊 使用场景

### 场景1：仅后台记录
```yaml
visitor_map:
  enabled: false  # 不显示地图
  clustrmaps_id: "your_id_here"  # 但仍记录数据
```

### 场景2：公开显示
```yaml
visitor_map:
  enabled: true   # 显示地图
  clustrmaps_id: "your_id_here"
  title: "访客地图"
  description: "感谢来自世界各地的访客！"
```

## 🎨 自定义样式

访客地图组件会自动适应您的网站主题，包括：
- 响应式设计
- 深色/浅色模式支持
- 与 al-folio 主题完美融合

## 📈 数据查看

- **公开模式**：访客可以看到地图和基本统计
- **后台模式**：您可以在 ClustrMaps 后台查看详细数据

## 🔧 故障排除

如果地图不显示：
1. 检查 `enabled` 是否为 `true`
2. 确认 `clustrmaps_id` 是否正确
3. 清除浏览器缓存后重新加载

## 📝 注意事项

- ClustrMaps 免费版有访问量限制
- 数据更新可能有延迟
- 建议定期检查后台数据准确性
