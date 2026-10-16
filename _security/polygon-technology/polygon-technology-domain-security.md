---
api_specs:
- filename: polygon-technology-openapi-generated.yml
  format: yaml
  label: Polygon Labs API
  slug: polygon-technology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-technology/refs/heads/main/openapi/_ae-authored/polygon-technology-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: polygon.technology
  spf: true
hosts:
- cert_expires: Jan 11 03:48:12 2027 GMT
  host: polygon.technology
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Polygon Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polygon Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Polygon Labs
provider_slug: polygon-technology
slug: polygon-technology-domain-security
source_filename: polygon-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polygon.technology\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 03:48:12 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: polygon.technology\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polygon-technology/refs/heads/main/security/polygon-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fintech
- Payments
- Blockchain
- Stablecoin
- DeveloperPlatform
---
