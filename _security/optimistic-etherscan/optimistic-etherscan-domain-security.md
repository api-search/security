---
api_specs:
- filename: optimistic-etherscan-openapi.yml
  format: yaml
  label: Optimism Etherscan API
  slug: optimistic-etherscan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimistic-etherscan/refs/heads/main/openapi/optimistic-etherscan-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: etherscan.io
  spf: true
hosts:
- cert_expires: Sep 20 03:43:38 2026 GMT
  host: optimistic.etherscan.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: docs.optimism.etherscan.io
  https: false
- cert_expires: Sep 20 03:43:38 2026 GMT
  host: api-optimistic.etherscan.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optimistic Etherscan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optimism Etherscan, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Optimism Etherscan
provider_slug: optimistic-etherscan
slug: optimistic-etherscan-domain-security
source_filename: optimistic-etherscan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: optimistic.etherscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:43:38 2026 GMT\n  hsts: false\n- host: docs.optimism.etherscan.io\n  https: false\n- host: api-optimistic.etherscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:43:38 2026 GMT\n  hsts: false\ndomains:\n- domain: etherscan.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optimistic-etherscan/refs/heads/main/security/optimistic-etherscan-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Blockchain
- Optimism
- Layer 2
- Ethereum
- EVM
- Web3
- Cryptocurrency
---
