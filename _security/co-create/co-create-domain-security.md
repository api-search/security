---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usecocreate.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cocrt.xyz
  spf: false
hosts:
- cert_expires: Sep 14 10:33:42 2026 GMT
  host: www.usecocreate.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: docs.usecocreate.io
  https: false
- host: api.cocrt.xyz
  https: false
kind: domain-security
layout: security
method: probed
name: Co Create Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Co:Create, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Co:Create
provider_slug: co-create
slug: co-create-domain-security
source_filename: co-create-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usecocreate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 10:33:42 2026 GMT\n  hsts: null\n- host: docs.usecocreate.io\n  https: false\n- host: api.cocrt.xyz\n  https: false\ndomains:\n- domain: usecocreate.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cocrt.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/co-create/refs/heads/main/security/co-create-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Web3
- Loyalty
- Rewards
- NFT
- Blockchain
- Polygon
- Tokens
- Community
- Crypto
---
