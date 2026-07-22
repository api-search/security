---
api_specs:
- filename: terminal-3-openapi.yml
  format: yaml
  label: Terminal 3 API
  slug: terminal-3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-3/refs/heads/main/openapi/terminal-3-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: terminal3.io
  spf: true
hosts:
- cert_expires: Sep  2 06:36:07 2026 GMT
  host: terminal3.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 05:38:06 2026 GMT
  host: staging.terminal3.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terminal 3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terminal 3, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Terminal 3
provider_slug: terminal-3
slug: terminal-3-domain-security
source_filename: terminal-3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: terminal3.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 06:36:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: staging.terminal3.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 05:38:06 2026 GMT\n  hsts: false\ndomains:\n- domain: terminal3.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terminal-3/refs/heads/main/security/terminal-3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity
- Decentralized Identity
- Verifiable Credentials
- OpenID Connect
- KYC
- AML
- Confidential Computing
- AI Agents
- Privacy
- Web3
- DID
---
