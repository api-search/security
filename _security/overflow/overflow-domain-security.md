---
api_specs:
- filename: overflow-openapi-original.json
  format: json
  label: Overflow Open API
  slug: overflow-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: overflow.co
  spf: true
hosts:
- cert_expires: Oct 10 20:49:22 2026 GMT
  host: docs.overflow.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: server.overflow.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: server.stage.overflow.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Overflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Overflow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Overflow
provider_slug: overflow
slug: overflow-domain-security
source_filename: overflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.overflow.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 20:49:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: server.overflow.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\n- host: server.stage.overflow.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: overflow.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/security/overflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Donations
- Fundraising
- Nonprofit
- Giving
- Recurring Payments
- Webhooks
- Cryptocurrency
---
