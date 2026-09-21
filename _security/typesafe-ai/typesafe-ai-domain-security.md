---
api_specs:
- filename: typesafe-ai-openapi.yml
  format: yaml
  label: TypeSafe System One API
  slug: system-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesafe-ai/refs/heads/main/openapi/typesafe-ai-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: typesafe.ai
  spf: true
hosts:
- cert_expires: Oct 23 00:21:18 2026 GMT
  host: typesafe.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 21:23:48 2026 GMT
  host: docs.typesafe.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 18:42:46 2026 GMT
  host: api.typesafe.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Typesafe Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TypeSafe AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: TypeSafe AI
provider_slug: typesafe-ai
slug: typesafe-ai-domain-security
source_filename: typesafe-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: typesafe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 00:21:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.typesafe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 21:23:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.typesafe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 18:42:46 2026 GMT\n  hsts: null\ndomains:\n- domain: typesafe.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typesafe-ai/refs/heads/main/security/typesafe-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Machine-Learning
- Classification
- Content Moderation
- Decision Support
- Structured Outputs
- Inference
- LLM Alternative
- Agent Skills
- MCP
- agent-native
- Developer Tools
---
