---
api_specs:
- filename: obie-opendata-swagger.json
  format: json
  label: UK Open Banking Open Data API (OBIE Standard)
  slug: uk-open-banking-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recognise-bank/refs/heads/main/openapi/obie-opendata-swagger.json
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: UK Open Banking Account & Transaction Information API (OBIE Standard)
  slug: uk-open-banking-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recognise-bank/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: UK Open Banking Payment Initiation API (OBIE Standard)
  slug: uk-open-banking-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recognise-bank/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: UK Open Banking Confirmation of Funds API (OBIE Standard)
  slug: uk-open-banking-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recognise-bank/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: recognisebank.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openbanking.org.uk
  spf: true
hosts:
- cert_expires: Sep 26 15:05:38 2026 GMT
  host: recognisebank.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.openbanking.org.uk
  https: false
kind: domain-security
layout: security
method: probed
name: Recognise Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recognise Bank, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Recognise Bank
provider_slug: recognise-bank
slug: recognise-bank-domain-security
source_filename: recognise-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: recognisebank.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:05:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.openbanking.org.uk\n  https: false\ndomains:\n- domain: recognisebank.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openbanking.org.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recognise-bank/refs/heads/main/security/recognise-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Savings
- SME Lending
- Fintech
- Account Information
---
