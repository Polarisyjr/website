# 访客地图设置指南

## https://clustrmaps.com/site/1c89n

一个简单的访客地图，显示在主页底部，记录访客的地理位置。

## ⚙️ 配置方法

在 `_config.yml` 文件中：

```yaml
visitor_map:
  enabled: true  # true=显示地图，false=仅后台记录
  clustrmaps_id: "R1Ulqk2j1x0ZQxF8b-_XgtkcLc17W9BKT-QWA88CsKM"  # 您的ID
```

## 📝 获取 ClustrMaps ID

1. 访问 [ClustrMaps.com](https://clustrmaps.com/)
2. 注册免费账户并添加您的网站
3. 复制代码中 `d=` 后面的 ID
4. 粘贴到配置文件的 `clustrmaps_id` 字段

## 📊 两种模式

**显示地图**（当前）：
```yaml
enabled: true  # 访客可以看到地图
```

**仅后台记录**：
```yaml
enabled: false  # 访客看不到，但数据照常记录
```

## 🔗 查看数据

访问 ClustrMaps 后台查看详细统计：
https://clustrmaps.com/site/R1Ulqk2j1x0ZQxF8b-_XgtkcLc17W9BKT-QWA88CsKM

就这么简单！
