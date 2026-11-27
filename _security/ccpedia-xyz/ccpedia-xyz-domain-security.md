---
api_specs:
- filename: ccpedia-xyz-openapi.yml
  format: yaml
  label: CCPEDIA REST API
  slug: ccpedia-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ccpedia-xyz/openapi/ccpedia-xyz-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ccpedia.xyz
  spf: false
hosts:
- cert_expires: Dec  5 18:19:59 2026 GMT
  host: ccpedia.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CCPEDIA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CCPEDIA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CCPEDIA
provider_slug: ccpedia-xyz
slug: ccpedia-xyz-domain-security
source_filename: ccpedia-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ccpedia.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 18:19:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ccpedia.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ccpedia-xyz/security/ccpedia-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Blockchain
- Knowledge Hub
- Canton Network
- Open Data
---
