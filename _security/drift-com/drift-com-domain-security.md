---
api_specs:
- filename: drift-com-openapi.yml
  format: yaml
  label: Drift REST API
  slug: drift-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: drift.com
  spf: true
hosts:
- cert_expires: Sep 26 20:17:29 2026 GMT
  host: www.drift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: app.drift.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 22:42:51 2026 GMT
  host: devdocs.drift.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drift Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drift, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Drift
provider_slug: drift-com
slug: drift-com-domain-security
source_filename: drift-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 20:17:29 2026 GMT\n  hsts: false\n- host: app.drift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: devdocs.drift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:42:51 2026 GMT\n  hsts: null\ndomains:\n- domain: drift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/security/drift-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Conversational Marketing
- Chatbots
- Sales
- Messaging
- Customer Engagement
- Revenue Orchestration
- AI Chat
---
