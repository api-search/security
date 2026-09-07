---
api_specs:
- filename: openapi.json
  format: json
  label: CommsHarbor API
  slug: commsharbor-api
  spec_type: OpenAPI
  url: https://commsharbor.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: commsharbor.com
  spf: false
hosts:
- cert_expires: Nov 27 08:14:51 2026 GMT
  host: commsharbor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Commsharbor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CommsHarbor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CommsHarbor
provider_slug: commsharbor
slug: commsharbor-domain-security
source_filename: commsharbor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commsharbor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 08:14:51 2026 GMT\n  hsts: false\ndomains:\n- domain: commsharbor.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/security/commsharbor-domain-security.yml
summary_line: TLSv1.3
tags:
- Email
- Transactional Email
- Email Marketing
- Communications
- Messaging
- Deliverability
- CRM
- Multi-tenant SaaS
- Agent-native
- MCP
- Web3 payments
- x402
---
