---
api_specs:
- filename: tsb-bank-atm-api-openapi.yml
  format: yaml
  label: TSB Bank ATM API
  slug: tsb-bank-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-atm-api-openapi.yml
- filename: tsb-bank-authorization-server-apis-api-openapi.yml
  format: yaml
  label: TSB Bank Authorization Server APIs API
  slug: tsb-bank-authorization-server-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-authorization-server-apis-api-openapi.yml
- filename: tsb-bank-bca-api-openapi.yml
  format: yaml
  label: TSB Bank BCA API
  slug: tsb-bank-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-bca-api-openapi.yml
- filename: tsb-bank-branch-api-openapi.yml
  format: yaml
  label: TSB Bank Branch API
  slug: tsb-bank-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-branch-api-openapi.yml
- filename: tsb-bank-ccc-api-openapi.yml
  format: yaml
  label: TSB Bank CCC API
  slug: tsb-bank-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-ccc-api-openapi.yml
- filename: tsb-bank-pca-api-openapi.yml
  format: yaml
  label: TSB Bank PCA API
  slug: tsb-bank-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-pca-api-openapi.yml
- filename: tsb-bank-resource-server-apis-api-openapi.yml
  format: yaml
  label: TSB Bank Resource Server APIs API
  slug: tsb-bank-resource-server-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-resource-server-apis-api-openapi.yml
- filename: tsb-bank-sme-api-openapi.yml
  format: yaml
  label: TSB Bank SME API
  slug: tsb-bank-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-sme-api-openapi.yml
- filename: tsb-bank-token-server-apis-api-openapi.yml
  format: yaml
  label: TSB Bank Token Server APIs API
  slug: tsb-bank-token-server-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-token-server-apis-api-openapi.yml
description: ''
domains:
- caa:
  - 128 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tsb.co.uk
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.tsb.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: apis.tsb.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: apis.developer.tsb.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tsb Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TSB Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: TSB Bank
provider_slug: tsb-bank
slug: tsb-bank-domain-security
source_filename: tsb-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tsb.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\n- host: apis.tsb.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: null\n- host: apis.developer.tsb.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tsb.co.uk\n  dnssec: true\n  caa:\n  - 128 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/security/tsb-bank-domain-security.yml
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
- FAPI
- Fintech
---
