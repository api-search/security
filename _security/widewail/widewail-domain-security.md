---
api_specs:
- filename: widewail-openapi-generated.yml
  format: yaml
  label: Widewail API
  slug: widewail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/widewail/openapi/_ae-authored/widewail-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: widewail.com
  spf: true
hosts:
- cert_expires: Jan 16 07:05:22 2027 GMT
  host: widewail.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Widewail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Widewail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Widewail
provider_slug: widewail
slug: widewail-domain-security
source_filename: widewail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: widewail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 07:05:22 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: widewail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/widewail/security/widewail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Customer Intelligence
- Software-as-a-Service
- Reputation Management
---
