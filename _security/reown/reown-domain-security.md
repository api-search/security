---
api_specs:
- filename: reown-openapi.yml
  format: yaml
  label: Reown Cloud Explorer API
  slug: explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reown/refs/heads/main/openapi/reown-openapi.yml
- filename: reown-asyncapi.yml
  format: yaml
  label: WalletConnect Relay (SDK-mediated)
  slug: walletconnect-protocol
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/reown/refs/heads/main/asyncapi/reown-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reown.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: web3modal.org
  spf: true
hosts:
- cert_expires: Sep  4 02:35:40 2026 GMT
  host: reown.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 20:11:33 2026 GMT
  host: docs.reown.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 21:58:10 2026 GMT
  host: api.web3modal.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reown Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reown, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reown
provider_slug: reown
slug: reown-domain-security
source_filename: reown-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reown.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:35:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.reown.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 20:11:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.web3modal.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 21:58:10 2026 GMT\n  hsts: null\ndomains:\n- domain: reown.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: web3modal.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reown/refs/heads/main/security/reown-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Wallets
- WalletConnect
- AppKit
- RPC
---
