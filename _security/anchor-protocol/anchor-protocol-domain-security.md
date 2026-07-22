---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anchorprotocol.com
  spf: true
hosts:
- cert_expires: Sep  1 22:48:02 2026 GMT
  host: anchorprotocol.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anchor Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anchor Protocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anchor Protocol
provider_slug: anchor-protocol
slug: anchor-protocol-domain-security
source_filename: anchor-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anchorprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 22:48:02 2026 GMT\n  hsts: null\ndomains:\n- domain: anchorprotocol.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchor-protocol/refs/heads/main/security/anchor-protocol-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- DeFi
- Blockchain
- Web3
- Savings
- Lending
- Terra
- Smart Contracts
---
