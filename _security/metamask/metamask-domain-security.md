---
api_specs:
- filename: metamask-token-api-openapi.yml
  format: yaml
  label: MetaMask Token API
  slug: metamask-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metamask/refs/heads/main/openapi/metamask-token-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: metamask.io
  spf: true
hosts:
- cert_expires: Dec 24 11:13:07 2026 GMT
  host: metamask.io
  hsts: true
  hsts_max_age: 15778476
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Metamask Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MetaMask, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MetaMask
provider_slug: metamask
slug: metamask-domain-security
source_filename: metamask-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metamask.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 11:13:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15778476\ndomains:\n- domain: metamask.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metamask/refs/heads/main/security/metamask-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Wallets
- Web3
- Developer Tools
---
