---
description: ''
domains:
- caa:
  - 0 iodef "mailto:services@snxdao.io"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: synthetix.io
  spf: true
hosts:
- cert_expires: Sep 19 15:19:58 2026 GMT
  host: developers.synthetix.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: papi.synthetix.io
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: api.synthetix.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Synthetix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synthetix, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Synthetix
provider_slug: synthetix
slug: synthetix-domain-security
source_filename: synthetix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.synthetix.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:19:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: papi.synthetix.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\n- host: api.synthetix.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: synthetix.io\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:services@snxdao.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthetix/refs/heads/main/security/synthetix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Derivatives
- Perpetuals
- Synthetic Assets
- Liquidity Protocol
- Blockchain
- Ethereum
- Optimism
- Base
- Trading
---
