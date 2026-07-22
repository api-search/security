---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: slingshot.finance
  spf: true
hosts:
- cert_expires: Sep 26 04:37:39 2026 GMT
  host: slingshot.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slingshot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slingshot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Slingshot
provider_slug: slingshot
slug: slingshot-domain-security
source_filename: slingshot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: slingshot.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 04:37:39 2026 GMT\n  hsts: null\ndomains:\n- domain: slingshot.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slingshot/refs/heads/main/security/slingshot-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Defi
- Cryptocurrency
- Wallet
- Trading
- Web3
- Blockchain
- Self-Custody
---
