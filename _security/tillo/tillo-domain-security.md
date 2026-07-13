---
api_specs:
- filename: tillo-gift-card-openapi.yml
  format: yaml
  label: Tillo Gift Card API
  slug: tillo-gift-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tillo/refs/heads/main/openapi/tillo-gift-card-openapi.yml
- filename: tillo-gift-card-openapi.yml
  format: yaml
  label: Tillo Float Management API
  slug: tillo-float-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tillo/refs/heads/main/openapi/tillo-gift-card-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tillo.io
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tillo.tech
  spf: true
hosts:
- cert_expires: Sep 21 17:33:35 2026 GMT
  host: www.tillo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: app.tillo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: tillo.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tillo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tillo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Tillo
provider_slug: tillo
slug: tillo-domain-security
source_filename: tillo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tillo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 17:33:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.tillo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tillo.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tillo.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tillo.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tillo/refs/heads/main/security/tillo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Gift Cards
- Payments
- Rewards
- Incentives
---
