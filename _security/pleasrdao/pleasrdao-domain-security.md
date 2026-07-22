---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pleasr.org
  spf: false
hosts:
- cert_expires: Sep 16 00:16:07 2026 GMT
  host: pleasr.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pleasrdao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PleasrDAO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: PleasrDAO
provider_slug: pleasrdao
slug: pleasrdao-domain-security
source_filename: pleasrdao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pleasr.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 00:16:07 2026 GMT\n  hsts: false\ndomains:\n- domain: pleasr.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pleasrdao/refs/heads/main/security/pleasrdao-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- DAO
- Web3
- NFT
- Digital Art
- Blockchain
- Collectibles
- Decentralized Finance
---
