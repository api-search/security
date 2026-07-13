---
api_specs:
- filename: tratta-openapi.yml
  format: yaml
  label: Tratta API
  slug: tratta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/openapi/tratta-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tratta.io
  spf: true
hosts:
- cert_expires: Sep  7 16:45:05 2026 GMT
  host: www.tratta.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 17:55:45 2026 GMT
  host: docs.tratta.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.tratta.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tratta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tratta, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tratta
provider_slug: tratta
slug: tratta-domain-security
source_filename: tratta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tratta.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 16:45:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tratta.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:55:45 2026 GMT\n  hsts: false\n- host: api.tratta.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tratta.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/security/tratta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Collections
- Payments
- Debt Collection
- Fintech
---
