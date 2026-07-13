---
api_specs:
- filename: qwen-openapi.yml
  format: yaml
  label: DashScope (Alibaba Cloud Model Studio) API
  slug: dashscope
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwen/refs/heads/main/openapi/qwen-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 iodef "mailto:certificate-transparency@list.alibaba-inc.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qwen.ai
  spf: true
- caa:
  - 0 iodef "mailto:certificate-transparency@list.alibaba-inc.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alibabacloud.com
  spf: true
hosts:
- cert_expires: Mar 31 02:36:11 2027 GMT
  host: qwen.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 02:26:16 2026 GMT
  host: www.alibabacloud.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  2 08:06:18 2026 GMT
  host: dashscope-intl.aliyuncs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qwen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qwen, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qwen
provider_slug: qwen
slug: qwen-domain-security
source_filename: qwen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qwen.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 31 02:36:11 2027 GMT\n  hsts: null\n- host: www.alibabacloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  5 02:26:16 2026 GMT\n  hsts: null\n- host: dashscope-intl.aliyuncs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:06:18 2026 GMT\n  hsts: null\ndomains:\n- domain: qwen.ai\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 iodef \"mailto:certificate-transparency@list.alibaba-inc.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: alibabacloud.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:certificate-transparency@list.alibaba-inc.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwen/refs/heads/main/security/qwen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- LLM
- Inference
- Open Source
- Alibaba
- Multimodal
---
