---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: redstone.finance
  spf: true
hosts:
- cert_expires: Aug 22 11:26:31 2026 GMT
  host: www.redstone.finance
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 11:26:31 2026 GMT
  host: docs.redstone.finance
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.redstone.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redstone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RedStone, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RedStone
provider_slug: redstone
slug: redstone-domain-security
source_filename: redstone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redstone.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 11:26:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.redstone.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 11:26:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.redstone.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: redstone.finance\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redstone/refs/heads/main/security/redstone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure
- Blockchain
- Oracle
- DeFi
- Price Feeds
- Data
- Web3
- Smart Contracts
---
