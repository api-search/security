---
api_specs:
- filename: centrifuge-openapi-generated.yml
  format: yaml
  label: Centrifuge API
  slug: centrifuge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centrifuge/openapi/_ae-authored/centrifuge-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: centrifuge.io
  spf: true
hosts:
- cert_expires: Jan 16 12:20:44 2027 GMT
  host: centrifuge.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Centrifuge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centrifuge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Centrifuge
provider_slug: centrifuge
slug: centrifuge-domain-security
source_filename: centrifuge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: centrifuge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 12:20:44 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: centrifuge.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/centrifuge/security/centrifuge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- DeFi
- Asset-Tokenization
- Blockchain
- FinTech
---
