---
api_specs:
- filename: openbanking-opendata-standard-swagger.json
  format: json
  label: Halifax Open Data ATM Locator API
  slug: halifax-open-data-atm-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/openbanking-opendata-standard-swagger.json
- filename: openbanking-opendata-standard-swagger.json
  format: json
  label: Halifax Open Data Branch Locator API
  slug: halifax-open-data-branch-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/openbanking-opendata-standard-swagger.json
- filename: openbanking-opendata-standard-swagger.json
  format: json
  label: Halifax Open Data Personal Current Accounts API
  slug: halifax-open-data-personal-current-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/openbanking-opendata-standard-swagger.json
- filename: openbanking-opendata-standard-swagger.json
  format: json
  label: Halifax Open Data Business Current Accounts API
  slug: halifax-open-data-business-current-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/openbanking-opendata-standard-swagger.json
- filename: openbanking-opendata-standard-swagger.json
  format: json
  label: Halifax Open Data Unsecured SME Loans API
  slug: halifax-open-data-unsecured-sme-loans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/openbanking-opendata-standard-swagger.json
- filename: openbanking-opendata-standard-swagger.json
  format: json
  label: Halifax Open Data Commercial Credit Cards API
  slug: halifax-open-data-commercial-credit-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/openbanking-opendata-standard-swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: halifax.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lloydsbanking.com
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: www.halifax.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: developer.lloydsbanking.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: api.halifax.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Halifax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Halifax, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Halifax
provider_slug: halifax
slug: halifax-domain-security
source_filename: halifax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.halifax.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.lloydsbanking.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.halifax.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: halifax.co.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lloydsbanking.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/security/halifax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
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
- Open Data
---
