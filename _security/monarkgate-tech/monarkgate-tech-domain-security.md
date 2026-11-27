---
api_specs:
- filename: monarkgate-tech-attest-api-openapi.yml
  format: yaml
  label: MONARK Attest API
  slug: monarkgate-tech-attest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monarkgate-tech/openapi/monarkgate-tech-attest-api-openapi.yml
- filename: monarkgate-tech-calibrate-api-openapi.yml
  format: yaml
  label: MONARK Calibrate API
  slug: monarkgate-tech-calibrate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monarkgate-tech/openapi/monarkgate-tech-calibrate-api-openapi.yml
- filename: monarkgate-tech-cascade-api-openapi.yml
  format: yaml
  label: MONARK Cascade API
  slug: monarkgate-tech-cascade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monarkgate-tech/openapi/monarkgate-tech-cascade-api-openapi.yml
- filename: monarkgate-tech-gate-api-openapi.yml
  format: yaml
  label: MONARK Gate API
  slug: monarkgate-tech-gate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monarkgate-tech/openapi/monarkgate-tech-gate-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: monarkgate.tech
  spf: true
hosts:
- cert_expires: Feb  7 01:32:15 2027 GMT
  host: monarkgate.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MONARK Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MONARK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MONARK
provider_slug: monarkgate-tech
slug: monarkgate-tech-domain-security
source_filename: monarkgate-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monarkgate.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 01:32:15 2027 GMT\n  hsts: false\ndomains:\n- domain: monarkgate.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/monarkgate-tech/security/monarkgate-tech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- DeFi
- Gatekeeping
- Platform
- Company
---
