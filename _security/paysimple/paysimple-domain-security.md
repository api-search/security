---
api_specs:
- filename: paysimple-openapi-generated.yml
  format: yaml
  label: PaySimple API
  slug: paysimple-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paysimple/openapi/_ae-authored/paysimple-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paysimple.com
  spf: true
hosts:
- cert_expires: Feb  8 07:16:25 2027 GMT
  host: paysimple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PaySimple Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PaySimple, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PaySimple
provider_slug: paysimple
slug: paysimple-domain-security
source_filename: paysimple-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paysimple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 07:16:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: paysimple.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/paysimple/security/paysimple-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Billing
- Software-as-a-Service
- Small Business
---
