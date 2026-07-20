---
api_specs:
- filename: gauntlet-openapi-original.json
  format: json
  label: Gauntlet API
  slug: gauntlet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gauntlet/refs/heads/main/openapi/gauntlet-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gauntlet.xyz
  spf: true
hosts:
- cert_expires: Sep  1 03:34:07 2026 GMT
  host: www.gauntlet.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 10:44:04 2026 GMT
  host: docs.gauntlet.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 10:45:13 2026 GMT
  host: api.gauntlet.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gauntlet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gauntlet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Gauntlet
provider_slug: gauntlet
slug: gauntlet-domain-security
source_filename: gauntlet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gauntlet.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 03:34:07 2026 GMT\n  hsts: false\n- host: docs.gauntlet.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 10:44:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gauntlet.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 10:45:13 2026 GMT\n  hsts: false\ndomains:\n- domain: gauntlet.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gauntlet/refs/heads/main/security/gauntlet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Data
- DeFi
- Risk Management
- Yield
- Vaults
- Blockchain
- Web3
- Financial Modeling
---
