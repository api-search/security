---
api_specs:
- filename: credo-ai-governance-platform-swagger.json
  format: json
  label: Credo AI Governance Platform API (v2)
  slug: credo-ai-governance-platform-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credo-ai/refs/heads/main/openapi/credo-ai-governance-platform-swagger.json
- filename: credo-ai-audit-logs-shadow-ai-openapi.json
  format: json
  label: Credo AI Audit Logs & Shadow AI API
  slug: credo-ai-audit-logs-shadow-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credo-ai/refs/heads/main/openapi/credo-ai-audit-logs-shadow-ai-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: credo.ai
  spf: true
hosts:
- cert_expires: Oct 26 01:11:29 2026 GMT
  host: www.credo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: docs.sdk.credo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.credo.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: 'Corrected by hand after the automated probe recorded hsts:null. A live `curl -I https://api.credo.ai/` on 2026-08-11 returns `strict-transport-security: max-age=63072000; includeSubDomains; preload`, as does an authenticated-path 401. The API host also returns x-content-type-options:nosniff, x-frame-options:DENY, a content-security-policy, referrer-policy:strict-origin-when-cross-origin, and an x-request-id correlation header.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Credo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credo AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Credo AI
provider_slug: credo-ai
slug: credo-ai-domain-security
source_filename: credo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.credo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 01:11:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sdk.credo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.credo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: >-\n    Corrected by hand after the automated probe recorded hsts:null. A live\n    `curl -I https://api.credo.ai/` on 2026-08-11 returns\n    `strict-transport-security: max-age=63072000; includeSubDomains; preload`,\n    as does an authenticated-path 401. The API host also returns\n    x-content-type-options:nosniff, x-frame-options:DENY, a\n    content-security-policy, referrer-policy:strict-origin-when-cross-origin,\n\
  \    and an x-request-id correlation header.\ndomains:\n- domain: credo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credo-ai/refs/heads/main/security/credo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- ai-governance
- ai-risk-management
- responsible-ai
- compliance
- regulatory-technology
- model-registry
- vendor-risk
- eu-ai-act
- nist-ai-rmf
- iso-42001
- shadow-ai
- agent-governance
- audit
- json-api
- agent-skills
---
