---
api_specs:
- filename: firenum-com-fire-plan-api-openapi.yml
  format: yaml
  label: firenum Fire Plan API
  slug: firenum-com-fire-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firenum-com/openapi/firenum-com-fire-plan-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: firenum.com
  spf: true
hosts:
- cert_expires: Jan 23 13:13:14 2027 GMT
  host: firenum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firenum Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for firenum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: firenum
provider_slug: firenum-com
slug: firenum-com-domain-security
source_filename: firenum-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firenum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 13:13:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: firenum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/firenum-com/security/firenum-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Retirement
- Calculator
- Free
- PersonalFinance
---
