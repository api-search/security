---
api_specs:
- filename: lorikeet-openapi.yml
  format: yaml
  label: Lorikeet Conversations API
  slug: lorikeet-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-openapi.yml
- filename: lorikeet-openapi.yml
  format: yaml
  label: Lorikeet Messages API
  slug: lorikeet-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-openapi.yml
- filename: lorikeet-openapi.yml
  format: yaml
  label: Lorikeet Webhooks & Events API
  slug: lorikeet-webhooks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-openapi.yml
- filename: lorikeet-openapi.yml
  format: yaml
  label: Lorikeet Actions & Tools API
  slug: lorikeet-actions-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-openapi.yml
- filename: lorikeet-openapi.yml
  format: yaml
  label: Lorikeet Knowledge Ingestion API
  slug: lorikeet-knowledge-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lorikeet.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lorikeetcx.ai
  spf: true
hosts:
- cert_expires: Sep 25 14:30:47 2026 GMT
  host: lorikeet.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:36:29 2026 GMT
  host: docs.lorikeetcx.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 20:59:37 2026 GMT
  host: api.lorikeetcx.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lorikeet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lorikeet, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lorikeet
provider_slug: lorikeet
slug: lorikeet-domain-security
source_filename: lorikeet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lorikeet.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:30:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lorikeetcx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:36:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lorikeetcx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 20:59:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lorikeet.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: lorikeetcx.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/security/lorikeet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Customer Support
- AI Agent
- Support Automation
- Workflows
- Helpdesk
---
