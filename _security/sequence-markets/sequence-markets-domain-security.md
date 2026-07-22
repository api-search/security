---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sequencemkts.com
  spf: true
hosts:
- cert_expires: Aug 26 01:38:40 2026 GMT
  host: sequencemkts.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 07:03:21 2026 GMT
  host: docs.sequencemkts.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 13:45:58 2026 GMT
  host: api.sequencemkts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sequence Markets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sequence Markets, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sequence Markets
provider_slug: sequence-markets
slug: sequence-markets-domain-security
source_filename: sequence-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sequencemkts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:38:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sequencemkts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 07:03:21 2026 GMT\n  hsts: false\n- host: api.sequencemkts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 13:45:58 2026 GMT\n  hsts: null\ndomains:\n- domain: sequencemkts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequence-markets/refs/heads/main/security/sequence-markets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Trading
- Cryptocurrency
- Digital Assets
- Execution
- Smart Order Routing
- Prediction Markets
- Algorithmic Trading
- DeFi
- Market Data
- FinTech
- Developer Tools
---
