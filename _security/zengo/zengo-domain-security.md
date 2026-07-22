---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zengo.com
  spf: true
hosts:
- cert_expires: Aug 26 01:10:14 2026 GMT
  host: www.zengo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zengo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZenGo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ZenGo
provider_slug: zengo
slug: zengo-domain-security
source_filename: zengo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zengo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:10:14 2026 GMT\n  hsts: null\ndomains:\n- domain: zengo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zengo/refs/heads/main/security/zengo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Cryptocurrency
- Wallet
- Web3
- Blockchain
- Security
- MPC
---
