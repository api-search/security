---
api_specs:
- filename: co-operative-bank-atm-api-openapi.yml
  format: yaml
  label: The Co-operative Bank ATM API
  slug: co-operative-bank-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-atm-api-openapi.yml
- filename: co-operative-bank-bca-api-openapi.yml
  format: yaml
  label: The Co-operative Bank BCA API
  slug: co-operative-bank-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-bca-api-openapi.yml
- filename: co-operative-bank-branch-api-openapi.yml
  format: yaml
  label: The Co-operative Bank Branch API
  slug: co-operative-bank-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-branch-api-openapi.yml
- filename: co-operative-bank-ccc-api-openapi.yml
  format: yaml
  label: The Co-operative Bank CCC API
  slug: co-operative-bank-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-ccc-api-openapi.yml
- filename: co-operative-bank-pca-api-openapi.yml
  format: yaml
  label: The Co-operative Bank PCA API
  slug: co-operative-bank-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-pca-api-openapi.yml
- filename: co-operative-bank-sme-api-openapi.yml
  format: yaml
  label: The Co-operative Bank SME API
  slug: co-operative-bank-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-sme-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: co-operativebank.co.uk
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: www.co-operativebank.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.developer.co-operativebank.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: openbanking-retail.apis.co-operativebank.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Co Operative Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Co-operative Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: The Co-operative Bank
provider_slug: co-operative-bank
slug: co-operative-bank-domain-security
source_filename: co-operative-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.co-operativebank.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.developer.co-operativebank.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openbanking-retail.apis.co-operativebank.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: co-operativebank.co.uk\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/security/co-operative-bank-domain-security.yml
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
- Confirmation of Funds
- Fintech
---
