---
api_specs:
- filename: contalink-openapi-original.json
  format: json
  label: Contalink API
  slug: contalink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contalink/refs/heads/main/openapi/contalink-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: contalink.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Aug 27 19:51:57 2026 GMT
  host: contalink.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 04:36:07 2026 GMT
  host: apidocs.contalink.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: 794lol2h95.execute-api.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Contalink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contalink, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Contalink
provider_slug: contalink
slug: contalink-domain-security
source_filename: contalink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contalink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:51:57 2026 GMT\n  hsts: false\n- host: apidocs.contalink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 04:36:07 2026 GMT\n  hsts: false\n- host: 794lol2h95.execute-api.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: contalink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contalink/refs/heads/main/security/contalink-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Accounting
- Bookkeeping
- Payroll
- Tax
- Fintech
- Invoicing
- CFDI
- Mexico
- SaaS
---
