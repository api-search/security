---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rtfkt.com
  spf: false
hosts:
- cert_expires: Oct  3 17:01:02 2026 GMT
  host: rtfkt.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rtfkt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RTFKT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: RTFKT
provider_slug: rtfkt
slug: rtfkt-domain-security
source_filename: rtfkt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rtfkt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:01:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: rtfkt.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rtfkt/refs/heads/main/security/rtfkt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Fashion
- NFT
- Collectibles
- Web3
- Metaverse
- Nike
- Consumer Brand
---
