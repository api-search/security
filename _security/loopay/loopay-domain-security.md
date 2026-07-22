---
api_specs:
- filename: loopay-openapi-original.json
  format: json
  label: Loopay API
  slug: loopay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: loopay.com
  spf: true
hosts:
- cert_expires: Sep 10 01:43:40 2026 GMT
  host: loopay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.loopay.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Loopay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loopay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Loopay
provider_slug: loopay
slug: loopay-domain-security
source_filename: loopay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loopay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 01:43:40 2026 GMT\n  hsts: false\n- host: api.loopay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: loopay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/security/loopay-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Payments
- Fintech
- Banking as a Service
- Cross-Border Payments
- Payouts
- Treasury
- Latin America
---
