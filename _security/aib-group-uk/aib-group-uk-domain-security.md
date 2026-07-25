---
api_specs:
- filename: aib-group-uk-open-data-openapi.json
  format: json
  label: AIB Group (UK) Open Data API
  slug: aib-group-uk-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aib-group-uk/refs/heads/main/openapi/aib-group-uk-open-data-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aibgb.co.uk
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: www.aibgb.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: developer.aibgb.co.uk
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: openapi.aibgb.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Aib Group Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIB Group (UK), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AIB Group (UK)
provider_slug: aib-group-uk
slug: aib-group-uk-domain-security
source_filename: aib-group-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aibgb.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\n- host: developer.aibgb.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 1000\n- host: openapi.aibgb.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: aibgb.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aib-group-uk/refs/heads/main/security/aib-group-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- Northern Ireland
---
