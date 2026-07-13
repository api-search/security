---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alchemix.fi
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: drpc.org
  spf: true
hosts:
- cert_expires: Aug 20 10:10:28 2026 GMT
  host: docs.alchemix.fi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 00:00:59 2026 GMT
  host: ethereum.drpc.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 21:32:21 2026 GMT
  host: thegraph.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alchemix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alchemix, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Alchemix
provider_slug: alchemix
slug: alchemix-domain-security
source_filename: alchemix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.alchemix.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 10:10:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ethereum.drpc.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 00:00:59 2026 GMT\n  hsts: null\n- host: thegraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:32:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alchemix.fi\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: drpc.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alchemix/refs/heads/main/security/alchemix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Self-Repaying Loans
- Synthetic Assets
- Yield
- Ethereum
- Blockchain
- Lending
- alUSD
- alETH
- ALCX
---
