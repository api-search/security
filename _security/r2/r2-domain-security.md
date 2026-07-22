---
api_specs:
- filename: r2-openapi.json
  format: json
  label: R2 API
  slug: r2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/r2/refs/heads/main/openapi/r2-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: r2capital.co
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: gateway-dev.r2capital.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: R2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for R2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: R2
provider_slug: r2
slug: r2-domain-security
source_filename: r2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gateway-dev.r2capital.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: r2capital.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/r2/refs/heads/main/security/r2-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Embedded Finance
- Lending
- Payments
- Fintech
- Latin America
- Revenue-Based Financing
- Webhooks
---
