# 保险经纪人 AI 应用

> KK 的个人保险经纪人 AI 助手项目

## 结构

```
data/insurance/     # 产品数据库（KK 维护）
  _schema.yaml      # 数据格式规范
  _knowledge.yaml   # 通用Q&A知识库
  medical/          # 医疗险产品
skills/             # OpenClaw 技能
temp/               # 临时方案文件
```

## 组件

- **Data 层**：保险产品结构化数据（条款/费率/健告/服务/免责）
- **Skill 层**：insurance-broker 分析引擎
- **Agent 层**：小KK 对话服务

## 相关

- 保险经纪人：KK（明亚保险经纪）
