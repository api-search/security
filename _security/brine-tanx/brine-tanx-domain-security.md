---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tanx.fi
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: brine.fi
  spf: true
hosts:
- cert_expires: Sep  1 11:33:22 2026 GMT
  host: tanx.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 10:13:57 2026 GMT
  host: www.brine.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brine Tanx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brine (Tanx), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Brine (Tanx)
provider_slug: brine-tanx
slug: brine-tanx-domain-security
source_filename: brine-tanx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tanx.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:33:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.brine.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 10:13:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tanx.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: brine.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brine-tanx/refs/heads/main/security/brine-tanx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Decentralized Exchange
- DeFi
- Blockchain
- Trading
- StarkEx
- Cross-chain
---
