---
api_specs:
- filename: merge-hris-api-openapi.yaml
  format: yaml
  label: Merge HRIS API
  slug: hris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-hris-api-openapi.yaml
- filename: merge-ats-api-openapi.yaml
  format: yaml
  label: Merge ATS API
  slug: ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-ats-api-openapi.yaml
- filename: merge-accounting-api-openapi.yaml
  format: yaml
  label: Merge Accounting API
  slug: accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-accounting-api-openapi.yaml
- filename: merge-ticketing-api-openapi.yaml
  format: yaml
  label: Merge Ticketing API
  slug: ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-ticketing-api-openapi.yaml
- filename: merge-crm-api-openapi.yaml
  format: yaml
  label: Merge CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-crm-api-openapi.yaml
- filename: merge-file-storage-api-openapi.yaml
  format: yaml
  label: Merge File Storage API
  slug: file-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-file-storage-api-openapi.yaml
- filename: merge-knowledge-base-api-openapi.yaml
  format: yaml
  label: Merge Knowledge Base API
  slug: knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-knowledge-base-api-openapi.yaml
- filename: merge-chat-api-openapi.yaml
  format: yaml
  label: Merge Chat API
  slug: chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-chat-api-openapi.yaml
- filename: merge-agent-handler-api-openapi.yaml
  format: yaml
  label: Merge Agent Handler
  slug: agent-handler
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-agent-handler-api-openapi.yaml
- filename: merge-gateway-api-openapi.yaml
  format: yaml
  label: Merge Gateway
  slug: gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-gateway-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: merge.dev
  spf: true
hosts:
- cert_expires: Oct  2 04:33:26 2026 GMT
  host: www.merge.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:00:10 2026 GMT
  host: api.merge.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 17:26:34 2026 GMT
  host: ah-api.merge.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Merge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Merge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Merge
provider_slug: merge
slug: merge-domain-security
source_filename: merge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.merge.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:33:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.merge.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:00:10 2026 GMT\n  hsts: null\n- host: ah-api.merge.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 17:26:34 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: merge.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/security/merge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Integrations
- Platform
- Unified API
- Agent Handler
- LLM Gateway
---
