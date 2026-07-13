---
api_specs:
- filename: osmapi-chat-completions-openapi.yml
  format: yaml
  label: osmAPI Chat Completions API
  slug: osmapi-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/openapi/osmapi-chat-completions-openapi.yml
- filename: osmapi-anthropic-messages-openapi.yml
  format: yaml
  label: osmAPI Anthropic Messages API
  slug: osmapi-anthropic-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/openapi/osmapi-anthropic-messages-openapi.yml
- filename: osmapi-models-openapi.yml
  format: yaml
  label: osmAPI Models API
  slug: osmapi-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/openapi/osmapi-models-openapi.yml
- filename: osmapi-health-openapi.yml
  format: yaml
  label: osmAPI Health API
  slug: osmapi-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/openapi/osmapi-health-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: osmapi.com
  spf: true
hosts:
- cert_expires: Aug  8 20:55:18 2026 GMT
  host: www.osmapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 14:42:35 2026 GMT
  host: docs.osmapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 14:42:35 2026 GMT
  host: api.osmapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Osmapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for osmAPI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: osmAPI
provider_slug: osmapi
slug: osmapi-domain-security
source_filename: osmapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.osmapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 20:55:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.osmapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 14:42:35 2026 GMT\n  hsts: false\n- host: api.osmapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 14:42:35 2026 GMT\n  hsts: false\ndomains:\n- domain: osmapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/security/osmapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Anthropic
- Gateway
- LLM
- OpenAI
- Routing
---
