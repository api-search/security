---
api_specs:
- filename: amberflo-metering-openapi.yaml
  format: yaml
  label: Amberflo Metering API
  slug: metering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/openapi/amberflo-metering-openapi.yaml
- filename: amberflo-billing-openapi.yaml
  format: yaml
  label: Amberflo Billing API
  slug: billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/openapi/amberflo-billing-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amberflo.io
  spf: false
hosts:
- cert_expires: Aug 16 09:55:12 2026 GMT
  host: www.amberflo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 20:57:14 2026 GMT
  host: docs.amberflo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: app.amberflo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amberflo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amberflo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Amberflo
provider_slug: amberflo
slug: amberflo-domain-security
source_filename: amberflo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amberflo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 09:55:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.amberflo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:57:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.amberflo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: amberflo.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/security/amberflo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
---
