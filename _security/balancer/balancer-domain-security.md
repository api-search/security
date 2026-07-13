---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: balancer.fi
  spf: true
hosts:
- cert_expires: Sep  5 03:19:34 2026 GMT
  host: balancer.fi
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 20:35:35 2026 GMT
  host: docs.balancer.fi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 08:00:20 2026 GMT
  host: api-v3.balancer.fi
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Balancer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Balancer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Balancer
provider_slug: balancer
slug: balancer-domain-security
source_filename: balancer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: balancer.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 03:19:34 2026 GMT\n  hsts: null\n- host: docs.balancer.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 20:35:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-v3.balancer.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:00:20 2026 GMT\n  hsts: false\ndomains:\n- domain: balancer.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/balancer/refs/heads/main/security/balancer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- DeFi
- DEX
- AMM
- Liquidity
- Multi-chain
- GraphQL
- Smart Order Router
- Open Source
---
