---
api_specs:
- filename: obie-opendata-swagger.json
  format: json
  label: Monument Bank Open Data API
  slug: monument-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monument-bank/refs/heads/main/openapi/obie-opendata-swagger.json
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: Monument Bank Account and Transaction Information API
  slug: monument-account-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monument-bank/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: Monument Bank Payment Initiation API
  slug: monument-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monument-bank/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: Monument Bank Confirmation of Funds API
  slug: monument-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monument-bank/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: monument.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openbanking.org.uk
  spf: true
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: www.monument.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: api.monument.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.openbanking.org.uk
  https: false
kind: domain-security
layout: security
method: probed
name: Monument Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monument Bank, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Monument Bank
provider_slug: monument-bank
slug: monument-bank-domain-security
source_filename: monument-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.monument.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: false\n- host: api.monument.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: null\n- host: developer.openbanking.org.uk\n  https: false\ndomains:\n- domain: monument.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openbanking.org.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monument-bank/refs/heads/main/security/monument-bank-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Savings
- Challenger Bank
- Account Information
- Payments
---
