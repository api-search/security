---
api_specs:
- filename: truebiz-openapi-original.json
  format: json
  label: TrueBiz Web Presence Review API
  slug: truebiz-web-presence-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/openapi/truebiz-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: truebiz.io
  spf: true
hosts:
- cert_expires: Oct  7 11:54:45 2026 GMT
  host: truebiz.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truebiz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrueBiz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: TrueBiz
provider_slug: truebiz
slug: truebiz-domain-security
source_filename: truebiz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truebiz.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 11:54:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: truebiz.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/security/truebiz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Fraud Prevention
- Business Verification
- Merchant Risk
- KYB
- Underwriting
- Payments
- Monitoring
---
