---
api_specs:
- filename: reachware-inc-reachpay-openapi.yml
  format: yaml
  label: Reach Pay API
  slug: reach-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reachware-inc/refs/heads/main/openapi/reachware-inc-reachpay-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reachware.com
  spf: true
hosts:
- cert_expires: Aug 31 23:44:51 2026 GMT
  host: reachware.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 23:44:51 2026 GMT
  host: api.reachware.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reachware Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reachware Inc., probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reachware Inc.
provider_slug: reachware-inc
slug: reachware-inc-domain-security
source_filename: reachware-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reachware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:44:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.reachware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:44:51 2026 GMT\n  hsts: null\ndomains:\n- domain: reachware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reachware-inc/refs/heads/main/security/reachware-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- iPaaS
- Integration
- Fintech
- Payment Gateway
- Tokenization
- Saudi Arabia
---
