---
api_specs:
- filename: ascend-openapi-original.yml
  format: yaml
  label: Ascend API V1
  slug: ascend-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ascend/refs/heads/main/openapi/ascend-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: useascend.com
  spf: true
hosts:
- cert_expires: Sep  7 01:21:15 2026 GMT
  host: useascend.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 10:25:12 2026 GMT
  host: developers.useascend.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 17:31:25 2026 GMT
  host: api.useascend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ascend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ascend, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ascend
provider_slug: ascend
slug: ascend-domain-security
source_filename: ascend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: useascend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 01:21:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.useascend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 10:25:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.useascend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 17:31:25 2026 GMT\n  hsts: false\ndomains:\n- domain: useascend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ascend/refs/heads/main/security/ascend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Insurance
- InsurTech
- Payments
- Premium Financing
- Billing
- Invoicing
- Embedded Finance
- REST API
- Webhooks
---
