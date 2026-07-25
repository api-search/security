---
api_specs:
- filename: obie-open-data-standard-openapi.json
  format: json
  label: Secure Trust Bank Open Data API (OBIE Standard)
  slug: open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/secure-trust-bank/refs/heads/main/openapi/obie-open-data-standard-openapi.json
- filename: obie-account-info-standard-openapi.yaml
  format: yaml
  label: Secure Trust Bank Account & Transaction Information API (OBIE Read/Write, AIS)
  slug: account-transaction-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/secure-trust-bank/refs/heads/main/openapi/obie-account-info-standard-openapi.yaml
- filename: obie-payment-initiation-standard-openapi.yaml
  format: yaml
  label: Secure Trust Bank Payment Initiation API (OBIE Read/Write, PIS)
  slug: payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/secure-trust-bank/refs/heads/main/openapi/obie-payment-initiation-standard-openapi.yaml
- filename: obie-confirmation-of-funds-standard-openapi.yaml
  format: yaml
  label: Secure Trust Bank Confirmation of Funds API (OBIE Read/Write, CBPII)
  slug: confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/secure-trust-bank/refs/heads/main/openapi/obie-confirmation-of-funds-standard-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: securetrustbank.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openbanking.org.uk
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: www.securetrustbank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.openbanking.org.uk
  https: false
kind: domain-security
layout: security
method: probed
name: Secure Trust Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Secure Trust Bank, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Secure Trust Bank
provider_slug: secure-trust-bank
slug: secure-trust-bank-domain-security
source_filename: secure-trust-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.securetrustbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: null\n- host: developer.openbanking.org.uk\n  https: false\ndomains:\n- domain: securetrustbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: openbanking.org.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secure-trust-bank/refs/heads/main/security/secure-trust-bank-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Specialist Lender
- Savings
---
