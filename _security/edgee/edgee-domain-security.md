---
api_specs:
- filename: edgee-chat-api-openapi.yml
  format: yaml
  label: Edgee Chat API
  slug: edgee-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/openapi/edgee-chat-api-openapi.yml
- filename: edgee-compress-api-openapi.yml
  format: yaml
  label: Edgee Compress API
  slug: edgee-compress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/openapi/edgee-compress-api-openapi.yml
- filename: edgee-messages-api-openapi.yml
  format: yaml
  label: Edgee Messages API
  slug: edgee-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/openapi/edgee-messages-api-openapi.yml
- filename: edgee-models-api-openapi.yml
  format: yaml
  label: Edgee Models API
  slug: edgee-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/openapi/edgee-models-api-openapi.yml
- filename: edgee-responses-api-openapi.yml
  format: yaml
  label: Edgee Responses API
  slug: edgee-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/openapi/edgee-responses-api-openapi.yml
- filename: edgee-tokens-api-openapi.yml
  format: yaml
  label: Edgee Tokens API
  slug: edgee-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/openapi/edgee-tokens-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: edgee.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: edgee.io
  spf: false
hosts:
- cert_expires: Oct 25 18:02:51 2026 GMT
  host: www.edgee.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: edgee.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 16:23:38 2026 GMT
  host: api.edgee.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edgee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edgee, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Edgee
provider_slug: edgee
slug: edgee-domain-security
source_filename: edgee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.edgee.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 18:02:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: edgee.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.edgee.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 16:23:38 2026 GMT\n  hsts: null\ndomains:\n- domain: edgee.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: edgee.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/security/edgee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- LLM
- AI Gateway
- Agents
- Developer Tools
- Observability
- FinOps
- Edge Computing
- Cost Management
---
