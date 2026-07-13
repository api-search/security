---
api_specs:
- filename: civic-pass-customer-api.yaml
  format: yaml
  label: Civic Pass API
  slug: civic-pass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civic/refs/heads/main/openapi/civic-pass-customer-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: civic.com
  spf: true
hosts:
- cert_expires: Oct  8 01:33:37 2026 GMT
  host: www.civic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: app.civic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 21:31:48 2026 GMT
  host: docs.civic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Civic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Civic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Civic
provider_slug: civic
slug: civic-domain-security
source_filename: civic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.civic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:33:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.civic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.civic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:31:48 2026 GMT\n  hsts: false\ndomains:\n- domain: civic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civic/refs/heads/main/security/civic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Authentication
- Digital Identity
- Identity Verification
- KYC
- MCP
- OAuth
- Security
- Solana
- Web3
- Wallets
---
