---
api_specs:
- filename: obie-opendata-swagger.json
  format: json
  label: Shawbrook Open Data API (OBIE Standard, Unverified)
  slug: shawbrook-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shawbrook-bank/refs/heads/main/openapi/obie-opendata-swagger.json
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: Shawbrook Account & Transaction Information API (AIS, OBIE Standard, Unverified)
  slug: shawbrook-account-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shawbrook-bank/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: Shawbrook Payment Initiation API (PIS, OBIE Standard, Unverified)
  slug: shawbrook-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shawbrook-bank/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: Shawbrook Confirmation of Funds API (CBPII, OBIE Standard, Unverified)
  slug: shawbrook-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shawbrook-bank/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shawbrook.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openbanking.org.uk
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: www.shawbrook.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: standards.openbanking.org.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.openbanking.org.uk
  https: false
kind: domain-security
layout: security
method: probed
name: Shawbrook Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shawbrook Bank, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shawbrook Bank
provider_slug: shawbrook-bank
slug: shawbrook-bank-domain-security
source_filename: shawbrook-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shawbrook.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: standards.openbanking.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.openbanking.org.uk\n  https: false\ndomains:\n- domain: shawbrook.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: openbanking.org.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shawbrook-bank/refs/heads/main/security/shawbrook-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- Savings
- Specialist Lending
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
---
