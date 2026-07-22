---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mainframe.co
  spf: true
hosts:
- cert_expires: Aug 24 18:55:45 2026 GMT
  host: mainframe.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mainframe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mainframe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mainframe
provider_slug: mainframe
slug: mainframe-domain-security
source_filename: mainframe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mainframe.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:55:45 2026 GMT\n  hsts: false\ndomains:\n- domain: mainframe.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mainframe/refs/heads/main/security/mainframe-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- DeFi
- Blockchain
- Web3
- NFT
- Software Development
- Marketing
---
