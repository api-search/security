---
api_specs:
- filename: cdr-register-openapi.json
  format: json
  label: CDR Register API
  slug: cdr-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/openapi/cdr-register-openapi.json
- filename: cdr-energy-openapi.json
  format: json
  label: CDR Energy API
  slug: cdr-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/openapi/cdr-energy-openapi.json
- filename: cdr-energy-sdh-openapi.json
  format: json
  label: CDR Energy Secondary Data Holder API
  slug: cdr-energy-secondary-data-holder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/openapi/cdr-energy-sdh-openapi.json
- filename: cdr-common-openapi.json
  format: json
  label: CDR Common API
  slug: cdr-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/openapi/cdr-common-openapi.json
- filename: cdr-dcr-openapi.json
  format: json
  label: CDR Dynamic Client Registration API
  slug: cdr-dynamic-client-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/openapi/cdr-dcr-openapi.json
- filename: cdr-admin-openapi.json
  format: json
  label: CDR Admin API
  slug: cdr-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/openapi/cdr-admin-openapi.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cdr.gov.au
  spf: true
hosts:
- cert_expires: Aug 26 19:08:30 2026 GMT
  host: www.cdr.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: api.cdr.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cdr Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Consumer Data Right (Energy), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Consumer Data Right (Energy)
provider_slug: cdr-energy
slug: cdr-energy-domain-security
source_filename: cdr-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cdr.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 19:08:30 2026 GMT\n  hsts: null\n- host: api.cdr.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cdr.gov.au\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/security/cdr-energy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Consumer Data Right
- Open Energy
- Smart Metering
- DER
- Energy Markets
- Regulation
- Government
- Open Data
---
