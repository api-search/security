---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shipyardsoftware.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clipper.exchange
  spf: true
hosts:
- cert_expires: Sep 13 15:23:07 2026 GMT
  host: www.shipyardsoftware.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 13:47:27 2026 GMT
  host: docs.clipper.exchange
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: blade-api.sushi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shipyard Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shipyard Software, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shipyard Software
provider_slug: shipyard-software
slug: shipyard-software-domain-security
source_filename: shipyard-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shipyardsoftware.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 15:23:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.clipper.exchange\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:47:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: blade-api.sushi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: shipyardsoftware.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: clipper.exchange\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipyard-software/refs/heads/main/security/shipyard-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defi
- DEX
- Decentralized Exchange
- Cryptocurrency
- Trading
- Blockchain
- Web3
- Liquidity
- RFQ
---
