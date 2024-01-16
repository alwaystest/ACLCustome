Separated AI related rules.

```yaml
proxy-groups:
  - name: 💬 OpenAi
    type: select
    proxies:
      - 🚀 节点选择
      - 🇺🇲 美国节点
      - DIRECT
rule-providers:
  AI:
  type: http
  behavior: classical
  url: "https://raw.githubusercontent.com/alwaystest/ACLCustome/master/Ai.yaml"
  path: ./rule_providers/Ai.yaml
  interval: 86400

rules:
  # AI
  - RULE-SET,AI,💬 OpenAi
```
