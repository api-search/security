---
api_specs:
- filename: requesty-openapi.yml
  format: yaml
  label: Requesty Chat Completions API
  slug: requesty-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/requesty/refs/heads/main/openapi/requesty-openapi.yml
- filename: requesty-openapi.yml
  format: yaml
  label: Requesty Models API
  slug: requesty-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/requesty/refs/heads/main/openapi/requesty-openapi.yml
- filename: requesty-openapi.yml
  format: yaml
  label: Requesty Usage & Analytics API
  slug: requesty-usage-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/requesty/refs/heads/main/openapi/requesty-openapi.yml
- filename: requesty-openapi.yml
  format: yaml
  label: Requesty API Keys API
  slug: requesty-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/requesty/refs/heads/main/openapi/requesty-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: requesty.ai
  spf: true
hosts:
- cert_expires: Aug 22 05:03:58 2026 GMT
  host: www.requesty.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 08:14:35 2026 GMT
  host: docs.requesty.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: router.requesty.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Requesty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Requesty, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Requesty
provider_slug: requesty
slug: requesty-domain-security
source_filename: requesty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.requesty.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 05:03:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.requesty.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:14:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: router.requesty.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: requesty.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/requesty/refs/heads/main/security/requesty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- LLM
- Routing
- Gateway
- Observability
---
