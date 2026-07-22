---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dclimate.net
  spf: true
hosts:
- cert_expires: Sep 15 21:36:43 2026 GMT
  host: dclimate.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dclimate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dClimate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: dClimate
provider_slug: dclimate
slug: dclimate-domain-security
source_filename: dclimate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dclimate.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:36:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dclimate.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dclimate/refs/heads/main/security/dclimate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Climate Data
- Weather Data
- Geospatial
- Decentralized
- IPFS
- Data Marketplace
- Zarr
- STAC
---
