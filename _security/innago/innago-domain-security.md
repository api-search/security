---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Innago API
  slug: innago-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: innago.com
  spf: true
hosts:
- cert_expires: Oct  4 02:40:26 2026 GMT
  host: docs.innago.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: api-my.innago.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Innago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Innago, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Innago
provider_slug: innago
slug: innago-domain-security
source_filename: innago-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.innago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:40:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-my.innago.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: innago.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/security/innago-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Property Management
- Real Estate
- Leases
- Rent Collection
- Maintenance
- Tenants
- Invoicing
- Payments
---
