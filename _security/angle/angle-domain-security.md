---
api_specs:
- filename: angle-api-openapi.json
  format: json
  label: Angle API
  slug: angle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/angle/refs/heads/main/openapi/angle-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: angle.money
  spf: true
hosts:
- cert_expires: Oct  6 12:00:05 2026 GMT
  host: angle.money
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 12:00:05 2026 GMT
  host: api.angle.money
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api-staging.angle.money
  https: false
kind: domain-security
layout: security
method: probed
name: Angle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Angle, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Angle
provider_slug: angle
slug: angle-domain-security
source_filename: angle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: angle.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 12:00:05 2026 GMT\n  hsts: false\n- host: api.angle.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 12:00:05 2026 GMT\n  hsts: false\n- host: api-staging.angle.money\n  https: false\ndomains:\n- domain: angle.money\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angle/refs/heads/main/security/angle-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Stablecoins
- Decentralized Finance
- Blockchain
- Cryptocurrency
- Smart Contracts
- Ethereum
- SDK
---
