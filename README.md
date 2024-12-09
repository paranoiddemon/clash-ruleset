# Clash ruleset

## How to use

doc: https://lancellc.gitbook.io/clash/clash-config-file/rule-provider

- example:

copy and paste this to the `rule-providers` block of your clash config file.

```yaml
  ChatGPT:
    type: http
    behavior: classical
    url: "https://raw.githubusercontent.com/paranoiddemon/clash-ruleset/main/ruleset/ai.yaml"
    path: ./ruleset/ai.yaml
    interval: 86400
```

then in the `rules` block:

```yaml
  - RULE-SET,ai,Proxy
```


