---
api_specs:
- filename: cynergy-bank-account-information-obie-standard-openapi.yaml
  format: yaml
  label: Cynergy Bank Account & Transaction Information API (AIS)
  slug: cynergy-bank-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cynergy-bank/refs/heads/main/openapi/cynergy-bank-account-information-obie-standard-openapi.yaml
- filename: cynergy-bank-payment-initiation-obie-standard-openapi.yaml
  format: yaml
  label: Cynergy Bank Payment Initiation API (PIS)
  slug: cynergy-bank-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cynergy-bank/refs/heads/main/openapi/cynergy-bank-payment-initiation-obie-standard-openapi.yaml
- filename: cynergy-bank-confirmation-of-funds-obie-standard-openapi.yaml
  format: yaml
  label: Cynergy Bank Confirmation of Funds API (CBPII)
  slug: cynergy-bank-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cynergy-bank/refs/heads/main/openapi/cynergy-bank-confirmation-of-funds-obie-standard-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cynergybank.co.uk
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: www.cynergybank.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: developer.openbanking.cynergybank.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cynergy Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cynergy Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cynergy Bank
provider_slug: cynergy-bank
slug: cynergy-bank-domain-security
source_filename: cynergy-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cynergybank.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.openbanking.cynergybank.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cynergybank.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cynergy-bank/refs/heads/main/security/cynergy-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- Specialist Lender
---
