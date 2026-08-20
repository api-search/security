---
api_specs:
- filename: uk-open-banking-account-info-api-openapi.yaml
  format: yaml
  label: GB Bank Account and Transaction Information API (AIS)
  slug: gb-bank-account-transaction-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gb-bank/refs/heads/main/openapi/uk-open-banking-account-info-api-openapi.yaml
- filename: uk-open-banking-payment-initiation-api-openapi.yaml
  format: yaml
  label: GB Bank Payment Initiation API (PIS)
  slug: gb-bank-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gb-bank/refs/heads/main/openapi/uk-open-banking-payment-initiation-api-openapi.yaml
- filename: uk-open-banking-confirmation-of-funds-api-openapi.yaml
  format: yaml
  label: GB Bank Confirmation of Funds API (CBPII)
  slug: gb-bank-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gb-bank/refs/heads/main/openapi/uk-open-banking-confirmation-of-funds-api-openapi.yaml
- filename: uk-open-banking-open-data-api-openapi.json
  format: json
  label: GB Bank Open Data API
  slug: uk-open-banking-open-data-api-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gb-bank/refs/heads/main/openapi/uk-open-banking-open-data-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gbbank.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openbanking.org.uk
  spf: true
hosts:
- cert_expires: Oct  9 11:22:49 2026 GMT
  host: www.gbbank.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.openbanking.org.uk
  https: false
kind: domain-security
layout: security
method: probed
name: Gb Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GB Bank, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GB Bank
provider_slug: gb-bank
slug: gb-bank-domain-security
source_filename: gb-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gbbank.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 11:22:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.openbanking.org.uk\n  https: false\ndomains:\n- domain: gbbank.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openbanking.org.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gb-bank/refs/heads/main/security/gb-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Savings
- Property Finance
- SME Lending
- Fintech
---
