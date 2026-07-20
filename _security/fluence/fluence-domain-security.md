---
api_specs:
- filename: fluence-openapi-original.yml
  format: yaml
  label: Fluence API
  slug: fluence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fluence.network
  spf: true
hosts:
- cert_expires: Oct  2 09:17:50 2026 GMT
  host: fluence.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fluence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fluence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fluence
provider_slug: fluence
slug: fluence-domain-security
source_filename: fluence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fluence.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 09:17:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fluence.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/security/fluence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Web3
- Cloud Compute
- DePIN
- GPU
- Infrastructure
- Virtual Machines
- AI Infrastructure
- Decentralized Cloud
---
