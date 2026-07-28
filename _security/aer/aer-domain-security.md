---
api_specs:
- filename: cdr-energy-api-openapi.json
  format: json
  label: AER Energy Product Reference Data - Get Generic Plans
  slug: aer-energy-product-reference-data-get-generic-plans
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/cdr-energy-api-openapi.json
- filename: cdr-energy-api-openapi.json
  format: json
  label: AER Energy Product Reference Data - Get Generic Plan Detail
  slug: aer-energy-product-reference-data-get-generic-plan-detail
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/cdr-energy-api-openapi.json
- filename: cds-common-api-openapi.json
  format: json
  label: AER CDR Discovery - Get Status and Get Outages
  slug: aer-cdr-discovery-status-and-outages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/cds-common-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aer.gov.au
  spf: true
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: energymadeeasy.gov.au
  spf: true
hosts:
- cert_expires: Oct  5 08:19:20 2026 GMT
  host: www.aer.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.energymadeeasy.gov.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: cdr.energymadeeasy.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australian Energy Regulator, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Australian Energy Regulator
provider_slug: aer
slug: aer-domain-security
source_filename: aer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aer.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 08:19:20 2026 GMT\n  hsts: null\n- host: www.energymadeeasy.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cdr.energymadeeasy.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: aer.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: energymadeeasy.gov.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/security/aer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Markets
- Consumer Data Right
- Retail Energy
- Regulation
- Government
- Open Data
- Smart Metering
---
