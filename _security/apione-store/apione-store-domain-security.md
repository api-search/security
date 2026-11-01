---
api_specs:
- filename: apione-store-openapi-generated.yml
  format: yaml
  label: apione-store API
  slug: apione-store-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apione-store/openapi/_ae-authored/apione-store-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apione.store
  spf: true
hosts:
- cert_expires: Jan 20 14:12:51 2027 GMT
  host: apione.store
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apione Store Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for apione-store, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: apione-store
provider_slug: apione-store
slug: apione-store-domain-security
source_filename: apione-store-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apione.store\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 14:12:51 2027 GMT\n  hsts: false\ndomains:\n- domain: apione.store\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/apione-store/security/apione-store-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- B2B
- Enrichment
- API
- Data
- GCC
- MENA
---
