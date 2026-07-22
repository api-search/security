---
api_specs:
- filename: syntage-openapi-original.yml
  format: yaml
  label: Syntage API
  slug: syntage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syntage/refs/heads/main/openapi/syntage-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: syntage.com
  spf: true
hosts:
- cert_expires: Sep 30 19:44:25 2026 GMT
  host: www.syntage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 13:46:11 2026 GMT
  host: api.syntage.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 11:17:53 2026 GMT
  host: api.sandbox.syntage.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Syntage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syntage, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Syntage
provider_slug: syntage
slug: syntage-domain-security
source_filename: syntage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.syntage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:44:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.syntage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 13:46:11 2026 GMT\n  hsts: false\n- host: api.sandbox.syntage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 11:17:53 2026 GMT\n  hsts: false\ndomains:\n- domain: syntage.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syntage/refs/heads/main/security/syntage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Mexico
- Credit Risk
- Financial Data
- KYC
- Compliance
- Invoices
- Factoring
- SAT
---
