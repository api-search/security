---
api_specs:
- filename: proto
  format: yaml
  label: XMTP Network gRPC API
  slug: xmtp-network-grpc-api
  spec_type: OpenAPI
  url: https://github.com/xmtp/proto
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: xmtp.org
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: xmtp.network
  spf: false
hosts:
- cert_expires: Oct  2 01:30:43 2026 GMT
  host: docs.xmtp.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: grpc.xmtp.network
  https: false
- host: xmtp.network
  https: false
kind: domain-security
layout: security
method: probed
name: Xmtp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XMTP, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: XMTP
provider_slug: xmtp
slug: xmtp-domain-security
source_filename: xmtp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.xmtp.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 01:30:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: grpc.xmtp.network\n  https: false\n- host: xmtp.network\n  https: false\ndomains:\n- domain: xmtp.org\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: xmtp.network\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xmtp/refs/heads/main/security/xmtp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Messaging
- Encryption
- Decentralized
- Ethereum
- MLS
- Wallets
- Agents
---
