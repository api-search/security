---
api_specs:
- filename: trustly-north-america-openapi.yml
  format: yaml
  label: Trustly North America API
  slug: trustly-north-america-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-north-america-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trustly.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: trustly.one
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.trustly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 03:06:38 2026 GMT
  host: amer.developers.trustly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: trustly.one
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Trustly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trustly Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trustly Group
provider_slug: trustly
slug: trustly-domain-security
source_filename: trustly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trustly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: amer.developers.trustly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 03:06:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: trustly.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trustly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: trustly.one\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/security/trustly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Pay by Bank
- Open Banking
- Account-to-Account
- Payouts
- Direct Debit
- Bank Account Verification
- Identity Verification
- Fintech
- Webhook
- MCP
---
