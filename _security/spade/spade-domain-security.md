---
api_specs:
- filename: spade-openapi-original.yml
  format: yaml
  label: Spade API
  slug: spade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spade/refs/heads/main/openapi/spade-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spade.com
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: east.sandbox.spade.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: east.api.spade.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: west.sandbox.spade.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Spade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spade, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spade
provider_slug: spade
slug: spade-domain-security
source_filename: spade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: east.sandbox.spade.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\n- host: east.api.spade.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\n- host: west.sandbox.spade.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: spade.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spade/refs/heads/main/security/spade-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Financial Services
- Transaction Enrichment
- Merchant Intelligence
- Payments
- Data Enrichment
- Fraud and Risk
- Fintech
---
