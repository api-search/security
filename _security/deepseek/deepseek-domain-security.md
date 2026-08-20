---
api_specs:
- filename: deepseek-chat-api-openapi.yml
  format: yaml
  label: DeepSeek Chat API
  slug: deepseek-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepseek/refs/heads/main/openapi/deepseek-chat-api-openapi.yml
- filename: deepseek-completions-api-openapi.yml
  format: yaml
  label: DeepSeek Completions API
  slug: deepseek-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepseek/refs/heads/main/openapi/deepseek-completions-api-openapi.yml
- filename: deepseek-models-api-openapi.yml
  format: yaml
  label: DeepSeek Models API
  slug: deepseek-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepseek/refs/heads/main/openapi/deepseek-models-api-openapi.yml
- filename: deepseek-user-api-openapi.yml
  format: yaml
  label: DeepSeek User API
  slug: deepseek-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepseek/refs/heads/main/openapi/deepseek-user-api-openapi.yml
description: ''
domains:
- caa:
  - d3bbv8sr76az5s.cloudfront.net.
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deepseek.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: www.deepseek.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: api-docs.deepseek.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.deepseek.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepseek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeepSeek, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DeepSeek
provider_slug: deepseek
slug: deepseek-domain-security
source_filename: deepseek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deepseek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\n- host: api-docs.deepseek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: false\n- host: api.deepseek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: deepseek.com\n  dnssec: false\n  caa:\n  - d3bbv8sr76az5s.cloudfront.net.\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepseek/refs/heads/main/security/deepseek-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Chat
- Chat Completion
- LLM
- Large Language Models
- Reasoning
- Code Completion
---
