---
api_specs:
- filename: rotessa-openapi.yml
  format: yaml
  label: Rotessa API
  slug: rotessa-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rotessa/refs/heads/main/openapi/rotessa-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rotessa.com
  spf: true
hosts:
- cert_expires: Oct 10 00:29:47 2026 GMT
  host: rotessa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 00:29:47 2026 GMT
  host: api.rotessa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 00:29:47 2026 GMT
  host: sandbox-api.rotessa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rotessa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rotessa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rotessa
provider_slug: rotessa
slug: rotessa-domain-security
source_filename: rotessa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rotessa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 00:29:47 2026 GMT\n  hsts: false\n- host: api.rotessa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 00:29:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sandbox-api.rotessa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 00:29:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rotessa.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rotessa/refs/heads/main/security/rotessa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Canada
- Pre-Authorized Debit
- ACH
- Account-to-Account
- Bank Payments
- Recurring Payments
- Subscription
- Direct Debit
- Money Movement
- Open Banking
---
