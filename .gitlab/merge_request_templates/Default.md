# [MR标题规范：类型] 简短描述 (关联ID)
<!-- 示例：[Feature] 用户登录支持OTP验证 (PROJ-123) -->

## 1. 变更类型
- [ ] 新功能 (Feature)
- [ ] 缺陷修复 (Bugfix) 
- [ ] 安全补丁 (Hotfix)
- [ ] 代码重构 (Refactor)
- [ ] 文档更新 (Docs)
- [ ] 其他 (请说明): _________

## 2. 关联工作项
<!-- 使用GitLab关键词实现自动化 -->
- 主Issue: Closes #123 
- 相关Issue: Related to #456, #789
- 需求文档: [Confluence链接](https://example.com)
- 原型设计: [Figma链接](https://example.com)

## 3. 变更描述
### 3.1 业务价值
<!-- 面向产品/业务人员说明 -->
> 允许用户通过短信/邮件接收一次性密码(OTP)登录，提升账户安全性

### 3.2 技术方案
```mermaid
sequenceDiagram
    participant 前端
    participant 后端
    participant 短信服务
    前端->>后端: 提交手机号/邮箱
    后端->>短信服务: 发送OTP(有效期5分钟)
    短信服务-->>后端: 发送状态
    后端-->>前端: 提示输入OTP
