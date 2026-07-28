---
api_specs:
- filename: energyaustralia-cds-energy-api-openapi.yml
  format: yaml
  label: EnergyAustralia CDR Energy Plans API
  slug: energyaustralia-cdr-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-cds-energy-api-openapi.yml
- filename: energyaustralia-cds-common-api-openapi.yml
  format: yaml
  label: EnergyAustralia CDR Discovery Status API
  slug: energyaustralia-cdr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-cds-common-api-openapi.yml
- filename: energyaustralia-cds-energy-api-openapi.yml
  format: yaml
  label: EnergyAustralia CDR Energy Consumer Data Sharing API
  slug: energyaustralia-cdr-energy-consumer-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-cds-energy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: energyaustralia.com.au
  spf: true
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: energymadeeasy.gov.au
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: www.energyaustralia.com.au
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
name: Energyaustralia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EnergyAustralia, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EnergyAustralia
provider_slug: energyaustralia
slug: energyaustralia-domain-security
source_filename: energyaustralia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.energyaustralia.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: null\n- host: www.energymadeeasy.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cdr.energymadeeasy.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: energyaustralia.com.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: energymadeeasy.gov.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/security/energyaustralia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retailer
- Consumer Data Right
- CDR
- Product Reference Data
- Smart Metering
- Energy Markets
- Renewables
---
