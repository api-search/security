---
api_specs:
- filename: frazzlecrm-com-openapi-generated.yml
  format: yaml
  label: FrazzleCRM API
  slug: frazzlecrm-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frazzlecrm-com/openapi/_ae-authored/frazzlecrm-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: frazzlecrm.com
  spf: true
hosts:
- cert_expires: Feb  2 05:12:45 2027 GMT
  host: frazzlecrm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 15:02:41 2026 GMT
  host: www.frazzlecrm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  9 15:03:01 2026 GMT
  host: app.frazzlecrm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: FrazzleCRM Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FrazzleCRM, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FrazzleCRM
provider_slug: frazzlecrm-com
slug: frazzlecrm-com-domain-security
source_filename: frazzlecrm-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frazzlecrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 05:12:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.frazzlecrm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  9 15:02:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.frazzlecrm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  9 15:03:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: frazzlecrm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/frazzlecrm-com/security/frazzlecrm-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- Automation
- Artificial Intelligence
- Software-as-a-Service
---
