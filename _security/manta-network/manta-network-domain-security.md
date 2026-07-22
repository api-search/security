---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "pki.goog"
  - 0 issuewildcard "amazontrust.com"
  - 0 issuewildcard "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: manta.network
  spf: true
hosts:
- cert_expires: Sep 23 23:56:51 2026 GMT
  host: manta.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Manta Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manta Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Manta Network
provider_slug: manta-network
slug: manta-network-domain-security
source_filename: manta-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manta.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:56:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: manta.network\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewildcard \"amazontrust.com\"\n  - 0 issuewildcard \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manta-network/refs/heads/main/security/manta-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Layer 2
- Blockchain
- Ethereum
- EVM
- Zero-Knowledge
- Polkadot
- Web3
- Modular Blockchain
- JSON-RPC
---
