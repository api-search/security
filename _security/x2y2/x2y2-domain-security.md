---
api_specs:
- filename: introduction
  format: yaml
  label: X2Y2 OpenAPI
  slug: x2y2-openapi
  spec_type: OpenAPI
  url: https://x2y2.readme.io/reference/introduction
- filename: introduction
  format: yaml
  label: X2Y2 Fi API
  slug: x2y2-fi-api
  spec_type: OpenAPI
  url: https://x2y2.readme.io/reference/introduction
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: x2y2.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: x2y2.org
  spf: true
hosts:
- cert_expires: Aug 24 07:47:08 2026 GMT
  host: docs.x2y2.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 21:28:39 2026 GMT
  host: api.x2y2.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 19:31:15 2026 GMT
  host: loan-api.x2y2.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: X2Y2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for X2Y2, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: X2Y2
provider_slug: x2y2
slug: x2y2-domain-security
source_filename: x2y2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.x2y2.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:47:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.x2y2.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 21:28:39 2026 GMT\n  hsts: null\n- host: loan-api.x2y2.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 19:31:15 2026 GMT\n  hsts: false\ndomains:\n- domain: x2y2.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: x2y2.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x2y2/refs/heads/main/security/x2y2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- NFT
- Ethereum
- Marketplace
- Blockchain
- Web3
- Collectibles
- Trading
---
