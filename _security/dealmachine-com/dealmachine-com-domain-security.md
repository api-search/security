---
api_specs:
- filename: dealmachine-com-openapi-generated.yml
  format: yaml
  label: DealMachine API
  slug: dealmachine-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealmachine-com/openapi/_ae-authored/dealmachine-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dealmachine.com
  spf: true
hosts:
- cert_expires: Jan  1 17:46:14 2027 GMT
  host: dealmachine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DealMachine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DealMachine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DealMachine
provider_slug: dealmachine-com
slug: dealmachine-com-domain-security
source_filename: dealmachine-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dealmachine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 17:46:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dealmachine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dealmachine-com/security/dealmachine-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Data
- Software-as-a-Service
- Lead Generation
- Property Search
---
