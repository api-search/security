---
api_specs:
- filename: ccbill-openapi-generated.yml
  format: yaml
  label: Ccbill API
  slug: ccbill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ccbill/openapi/_ae-authored/ccbill-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ccbill.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: ccbill.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ccbill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ccbill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ccbill
provider_slug: ccbill
slug: ccbill-domain-security
source_filename: ccbill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ccbill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ccbill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ccbill/security/ccbill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Merchant Services
- Billing
- Subscription
- E-Commerce
- Security
---
