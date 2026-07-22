---
api_specs:
- filename: methodfi-openapi-original.yml
  format: yaml
  label: Method API
  slug: method-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/methodfi/refs/heads/main/openapi/methodfi-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: methodfi.com
  spf: true
hosts:
- cert_expires: Aug 29 07:23:50 2026 GMT
  host: production.methodfi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 11 03:47:45 2026 GMT
  host: sandbox.methodfi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 11 03:48:09 2026 GMT
  host: dev.methodfi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Methodfi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MethodFi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MethodFi
provider_slug: methodfi
slug: methodfi-domain-security
source_filename: methodfi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: production.methodfi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 29 07:23:50 2026 GMT\n  hsts: null\n- host: sandbox.methodfi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 03:47:45 2026 GMT\n  hsts: null\n- host: dev.methodfi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 03:48:09 2026 GMT\n  hsts: null\ndomains:\n- domain: methodfi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/methodfi/refs/heads/main/security/methodfi-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fintech
- Liability Data
- Payments
- Lending
- Personal Finance
- Credit
- ACH
- Debt
- Identity Verification
---
