# 简单机器人示例

这是一个使用 omni-bot-sdk 的简单机器人示例。

## 配置说明

在运行机器人之前，你需要修改 `config.yaml` 文件中的以下配置：

### 必需配置

1. **dbkey**: 数据库加密密钥
   ```yaml
   dbkey: your_actual_database_key_here
   ```

2. **MQTT 配置**: 如果你使用 MQTT 功能
   ```yaml
   mqtt:
     password: 'your_actual_mqtt_password'
   ```

### 可选配置

- **钉钉机器人**: 如果需要异常通知
- **OpenAI 插件**: 如果需要 AI 对话功能
- **S3 存储**: 如果需要存储登录二维码

## 运行方法

```bash
python bot.py
```

## 注意事项

1. 确保你已经安装了所有必要的依赖
2. 根据你的实际需求修改配置文件
3. 首次运行可能需要设置数据库密钥
4. 如果遇到权限问题，请检查文件路径和权限设置 