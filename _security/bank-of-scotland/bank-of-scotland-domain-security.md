---
api_specs:
- filename: obie-opendata-swagger.json
  format: json
  label: Bank of Scotland Open Data API
  slug: bank-of-scotland-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-scotland/refs/heads/main/openapi/obie-opendata-swagger.json
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: Bank of Scotland Account and Transaction Information API (AIS)
  slug: bank-of-scotland-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-scotland/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: Bank of Scotland Payment Initiation API (PIS)
  slug: bank-of-scotland-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-scotland/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: Bank of Scotland Confirmation of Funds API (CBPII)
  slug: bank-of-scotland-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-scotland/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bankofscotland.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lloydsbanking.com
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: www.bankofscotland.co.uk
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
  host: api.bankofscotland.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bank Of Scotland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bank of Scotland, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bank of Scotland
provider_slug: bank-of-scotland
slug: bank-of-scotland-domain-security
source_filename: bank-of-scotland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bankofscotland.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.lloydsbanking.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bankofscotland.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bankofscotland.co.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lloydsbanking.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-scotland/refs/heads/main/security/bank-of-scotland-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
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
