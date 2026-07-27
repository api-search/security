---
api_specs:
- filename: itu-datahub-openapi.yml
  format: yaml
  label: ITU DataHub API
  slug: itu-datahub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itu/refs/heads/main/openapi/itu-datahub-openapi.yml
- filename: itu-proximity-openapi.yml
  format: yaml
  label: ITU Proximity to Fibre Node API
  slug: itu-proximity-to-fibre-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itu/refs/heads/main/openapi/itu-proximity-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: itu.int
  spf: true
hosts:
- cert_expires: Sep  9 00:50:38 2026 GMT
  host: www.itu.int
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: datahub.itu.int
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: api.datahub.itu.int
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Itu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ITU, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ITU
provider_slug: itu
slug: itu-domain-security
source_filename: itu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.itu.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 00:50:38 2026 GMT\n  hsts: false\n- host: datahub.itu.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: null\n- host: api.datahub.itu.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: itu.int\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itu/refs/heads/main/security/itu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Telecommunications
- Global
- Regulator
- Standards
- Spectrum
- Satellite
- Broadband
- ICT Statistics
- Open Data
- United Nations
---
