---
api_specs:
- filename: qiwi-openapi.yml
  format: yaml
  label: Qiwi Payment Protocol
  slug: qiwi-payment-protocol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qiwi/refs/heads/main/openapi/qiwi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qiwi.com
  spf: true
hosts:
- cert_expires: Oct 26 08:16:43 2026 GMT
  host: developer.qiwi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 08:16:43 2026 GMT
  host: qiwi.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 08:16:43 2026 GMT
  host: api.qiwi.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qiwi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qiwi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Qiwi
provider_slug: qiwi
slug: qiwi-domain-security
source_filename: qiwi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.qiwi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 08:16:43 2026 GMT\n  hsts: false\n- host: qiwi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 08:16:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.qiwi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 08:16:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: qiwi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qiwi/refs/heads/main/security/qiwi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Wallet
- Payouts
- Fintech
- Banking
---
