---
api_specs:
- filename: privy-openapi.yml
  format: yaml
  label: Privy REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privy/refs/heads/main/openapi/privy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: privy.io
  spf: true
hosts:
- cert_expires: Sep 18 22:02:54 2026 GMT
  host: www.privy.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 22:02:54 2026 GMT
  host: docs.privy.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 22:02:54 2026 GMT
  host: api.privy.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Privy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Privy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Privy
provider_slug: privy
slug: privy-domain-security
source_filename: privy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.privy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:02:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.privy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:02:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.privy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:02:54 2026 GMT\n  hsts: null\ndomains:\n- domain: privy.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/privy/refs/heads/main/security/privy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Wallets
- Authentication
- Embedded Wallets
- MPC
---
