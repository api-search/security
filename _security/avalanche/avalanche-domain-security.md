---
api_specs:
- filename: api
  format: yaml
  label: Avalanche Data API (Glacier)
  slug: avalanche-data-api-glacier
  spec_type: OpenAPI
  url: https://glacier-api.avax.network/api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: avacloud.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: avax.network
  spf: true
hosts:
- cert_expires: Aug 31 14:52:18 2026 GMT
  host: developers.avacloud.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 22:05:14 2026 GMT
  host: glacier-api.avax.network
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 22:05:14 2026 GMT
  host: build.avax.network
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avalanche Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avalanche, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Avalanche
provider_slug: avalanche
slug: avalanche-domain-security
source_filename: avalanche-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.avacloud.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 14:52:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: glacier-api.avax.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:05:14 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: build.avax.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:05:14 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: avacloud.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: avax.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avalanche/refs/heads/main/security/avalanche-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Web3
- Avalanche
- NFT
- DeFi
- Cross-Chain
---
