---
api_specs:
- filename: 3dpack-ing-packing-api-openapi.yml
  format: yaml
  label: 3dpack-ing Packing API
  slug: 3dpack-ing-packing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dpack-ing/openapi/3dpack-ing-packing-api-openapi.yml
- filename: 3dpack-ing-typed-api-openapi.yml
  format: yaml
  label: 3dpack-ing Typed API
  slug: 3dpack-ing-typed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dpack-ing/openapi/3dpack-ing-typed-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 3dpack.ing
  spf: true
hosts:
- cert_expires: Jan 15 09:44:41 2027 GMT
  host: 3dpack.ing
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 3Dpack Ing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3dpack-ing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 3dpack-ing
provider_slug: 3dpack-ing
slug: 3dpack-ing-domain-security
source_filename: 3dpack-ing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 3dpack.ing\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 09:44:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 3dpack.ing\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/3dpack-ing/security/3dpack-ing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- 3D
- API
- SaaS
---
