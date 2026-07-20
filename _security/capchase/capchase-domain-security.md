---
api_specs:
- filename: capchase-pay-openapi.yml
  format: yaml
  label: Capchase Pay API
  slug: capchase-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capchase/refs/heads/main/openapi/capchase-pay-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: capchase.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Oct  4 12:13:29 2026 GMT
  host: www.capchase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: capchase.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 15:14:51 2026 GMT
  host: universe.capchase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capchase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capchase, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Capchase
provider_slug: capchase
slug: capchase-domain-security
source_filename: capchase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.capchase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:13:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: capchase.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: universe.capchase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:14:51 2026 GMT\n  hsts: null\ndomains:\n- domain: capchase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capchase/refs/heads/main/security/capchase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Embedded Finance
- Financing
- B2B SaaS
- Revenue Financing
- BNPL
- KYB
- Underwriting
---
