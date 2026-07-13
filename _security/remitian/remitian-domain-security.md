---
api_specs:
- filename: remitian-tax-payment-openapi.yml
  format: yaml
  label: Remitian Tax Payment API
  slug: tax-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remitian/refs/heads/main/openapi/remitian-tax-payment-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: remitian.com
  spf: true
hosts:
- cert_expires: Sep  8 18:19:25 2026 GMT
  host: remitian.com
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: api.remitian.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Remitian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Remitian, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Remitian
provider_slug: remitian
slug: remitian-domain-security
source_filename: remitian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: remitian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 18:19:25 2026 GMT\n  hsts: true\n  hsts_max_age: 2628000\n- host: api.remitian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: remitian.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remitian/refs/heads/main/security/remitian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tax
- Payments
- Fintech
- Accounting
- Webhooks
- Embedded Payments
---
