---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eigenda.xyz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eigencloud.xyz
  spf: true
hosts:
- cert_expires: Aug 27 02:44:09 2026 GMT
  host: www.eigenda.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 19:07:07 2026 GMT
  host: eigencloud.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 19:07:07 2026 GMT
  host: docs.eigencloud.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eigenda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EigenDA, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EigenDA
provider_slug: eigenda
slug: eigenda-domain-security
source_filename: eigenda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eigenda.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 02:44:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: eigencloud.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:07:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.eigencloud.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:07:07 2026 GMT\n  hsts: null\ndomains:\n- domain: eigenda.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: eigencloud.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eigenda/refs/heads/main/security/eigenda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Data Availability
- Ethereum
- Restaking
- EigenLayer
- Rollups
- Layer 2
- Web3
- gRPC
- Decentralized Infrastructure
- KZG Commitments
- Cryptography
---
