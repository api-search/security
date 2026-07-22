---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zed.run
  spf: true
hosts:
- cert_expires: Sep  3 07:07:44 2026 GMT
  host: zed.run
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zedrun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zed.run, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zed.run
provider_slug: zedrun
slug: zedrun-domain-security
source_filename: zedrun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zed.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 07:07:44 2026 GMT\n  hsts: false\ndomains:\n- domain: zed.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zedrun/refs/heads/main/security/zedrun-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Blockchain
- NFT
- Web3
- Horse Racing
- Digital Collectibles
- Polygon
---
