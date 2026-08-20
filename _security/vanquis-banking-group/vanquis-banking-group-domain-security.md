---
api_specs:
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: Vanquis Bank Account and Transaction API (AIS)
  slug: vanquis-account-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanquis-banking-group/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: Vanquis Bank Payment Initiation API (PIS)
  slug: vanquis-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanquis-banking-group/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: Vanquis Bank Confirmation of Funds API (CBPII)
  slug: vanquis-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanquis-banking-group/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vanquis.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: vanquisbankinggroup.com
  spf: true
hosts:
- cert_expires: Aug 26 20:19:35 2026 GMT
  host: www.vanquis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:04:56 2026 GMT
  host: www.vanquisbankinggroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vanquis Banking Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vanquis Banking Group, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vanquis Banking Group
provider_slug: vanquis-banking-group
slug: vanquis-banking-group-domain-security
source_filename: vanquis-banking-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vanquis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:19:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.vanquisbankinggroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:04:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vanquis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: vanquisbankinggroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanquis-banking-group/refs/heads/main/security/vanquis-banking-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Specialist Lender
- Credit Cards
- Account Information
- Payments
---
