---
api_specs:
- filename: dexra-dev-api-openapi.json
  format: json
  label: Dexra Api API
  slug: dexra-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dexra-dev/openapi/_original/dexra-dev-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dexra.dev
  spf: true
hosts:
- cert_expires: Jan 15 11:15:59 2027 GMT
  host: dexra.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dexra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dexra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dexra
provider_slug: dexra-dev
slug: dexra-dev-domain-security
source_filename: dexra-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dexra.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 11:15:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dexra.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dexra-dev/security/dexra-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Artificial Intelligence
- Finance
- Data
- Solana
---
