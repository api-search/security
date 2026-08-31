---
api_specs:
- filename: metro-bank-atm-api-openapi.yml
  format: yaml
  label: Metro Bank ATM API
  slug: metro-bank-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/openapi/metro-bank-atm-api-openapi.yml
- filename: metro-bank-bca-api-openapi.yml
  format: yaml
  label: Metro Bank BCA API
  slug: metro-bank-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/openapi/metro-bank-bca-api-openapi.yml
- filename: metro-bank-branch-api-openapi.yml
  format: yaml
  label: Metro Bank Branch API
  slug: metro-bank-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/openapi/metro-bank-branch-api-openapi.yml
- filename: metro-bank-ccc-api-openapi.yml
  format: yaml
  label: Metro Bank CCC API
  slug: metro-bank-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/openapi/metro-bank-ccc-api-openapi.yml
- filename: metro-bank-pca-api-openapi.yml
  format: yaml
  label: Metro Bank PCA API
  slug: metro-bank-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/openapi/metro-bank-pca-api-openapi.yml
- filename: metro-bank-sme-api-openapi.yml
  format: yaml
  label: Metro Bank SME API
  slug: metro-bank-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/openapi/metro-bank-sme-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: metrobankonline.co.uk
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.metrobankonline.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 16:29:48 2026 GMT
  host: developer.metrobankonline.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: api.metrobankonline.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Metro Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metro Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Metro Bank
provider_slug: metro-bank
slug: metro-bank-domain-security
source_filename: metro-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.metrobankonline.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.metrobankonline.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:29:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.metrobankonline.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: metrobankonline.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/security/metro-bank-domain-security.yml
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
- FAPI
- Fintech
---
