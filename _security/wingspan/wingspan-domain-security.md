---
api_specs:
- filename: wingspan-payments-openapi-original.yml
  format: yaml
  label: Wingspan Payments API
  slug: wingspan-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-payments-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wingspan.app
  spf: true
hosts:
- cert_expires: Oct  5 12:24:59 2026 GMT
  host: api.wingspan.app
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 09:47:55 2026 GMT
  host: stagingapi.wingspan.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wingspan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wingspan, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wingspan
provider_slug: wingspan
slug: wingspan-domain-security
source_filename: wingspan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.wingspan.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:24:59 2026 GMT\n  hsts: null\n- host: stagingapi.wingspan.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:47:55 2026 GMT\n  hsts: null\ndomains:\n- domain: wingspan.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/security/wingspan-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Payroll
- Contractors
- Invoicing
- Taxes
- Fintech
- Freelance Economy
---
