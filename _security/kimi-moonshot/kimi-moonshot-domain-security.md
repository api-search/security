---
api_specs:
- filename: kimi-moonshot-batch-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Batch API
  slug: kimi-moonshot-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/openapi/kimi-moonshot-batch-api-openapi.yml
- filename: kimi-moonshot-billing-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Billing API
  slug: kimi-moonshot-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/openapi/kimi-moonshot-billing-api-openapi.yml
- filename: kimi-moonshot-chat-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Chat API
  slug: kimi-moonshot-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/openapi/kimi-moonshot-chat-api-openapi.yml
- filename: kimi-moonshot-files-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Files API
  slug: kimi-moonshot-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/openapi/kimi-moonshot-files-api-openapi.yml
- filename: kimi-moonshot-models-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Models API
  slug: kimi-moonshot-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/openapi/kimi-moonshot-models-api-openapi.yml
- filename: kimi-moonshot-utilities-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Utilities API
  slug: kimi-moonshot-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/openapi/kimi-moonshot-utilities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: moonshot.cn
  spf: true
hosts:
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: www.moonshot.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: platform.moonshot.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: api.moonshot.cn
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kimi Moonshot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kimi (Moonshot AI), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kimi (Moonshot AI)
provider_slug: kimi-moonshot
slug: kimi-moonshot-domain-security
source_filename: kimi-moonshot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moonshot.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.moonshot.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.moonshot.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: moonshot.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kimi-moonshot/refs/heads/main/security/kimi-moonshot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- LLM
- Long Context
- Artificial Intelligence
- OpenAI-Compatible
- Multimodal
- China
---
