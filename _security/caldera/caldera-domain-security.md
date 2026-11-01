---
api_specs:
- filename: caldera-openapi-generated.yml
  format: yaml
  label: Caldera API
  slug: caldera-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caldera/openapi/_ae-authored/caldera-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: caldera.xyz
  spf: true
hosts:
- cert_expires: Jan 13 06:55:09 2027 GMT
  host: caldera.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caldera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caldera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Caldera
provider_slug: caldera
slug: caldera-domain-security
source_filename: caldera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caldera.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 06:55:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: caldera.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/caldera/security/caldera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Interoperability
- Ethereum
- DeFi
- Platform
---
