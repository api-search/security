---
api_specs:
- filename: preauth-instacash-orders-openapi.yml
  format: yaml
  label: Preauth Orders API
  slug: preauth-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preauth-instacash/refs/heads/main/openapi/preauth-instacash-orders-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: preauth.io
  spf: true
hosts:
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: preauth.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 10:11:22 2026 GMT
  host: docs.preauth.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: api.preauth.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Preauth Instacash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PreAuth (Instacash), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PreAuth (Instacash)
provider_slug: preauth-instacash
slug: preauth-instacash-domain-security
source_filename: preauth-instacash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: preauth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: false\n- host: docs.preauth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 10:11:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.preauth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: preauth.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preauth-instacash/refs/heads/main/security/preauth-instacash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Payment Pre-Authorization
- Payment Guarantees
- Fintech
- Latin America
- Cards
---
