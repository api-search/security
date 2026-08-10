---
api_specs:
- filename: 73-strings-asset-info-api-openapi.yml
  format: yaml
  label: 73 Strings Asset Info API
  slug: 73-strings-asset-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-asset-info-api-openapi.yml
- filename: 73-strings-captable-api-openapi.yml
  format: yaml
  label: 73 Strings Captable API
  slug: 73-strings-captable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-captable-api-openapi.yml
- filename: 73-strings-documents-api-openapi.yml
  format: yaml
  label: 73 Strings Documents API
  slug: 73-strings-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-documents-api-openapi.yml
- filename: 73-strings-financial-data-api-openapi.yml
  format: yaml
  label: 73 Strings Financial Data API
  slug: 73-strings-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-financial-data-api-openapi.yml
- filename: 73-strings-qualitative-data-api-openapi.yml
  format: yaml
  label: 73 Strings Qualitative Data API
  slug: 73-strings-qualitative-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-qualitative-data-api-openapi.yml
- filename: 73-strings-transaction-api-api-openapi.yml
  format: yaml
  label: 73 Strings Transaction API API
  slug: 73-strings-transaction-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-transaction-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "letsencrypt.org,digicert.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: 73strings.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azure-api.net
  spf: false
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.73strings.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 21:42:13 2027 GMT
  host: api-accord-eut-73strings.developer.azure-api.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 21:42:13 2027 GMT
  host: api-accord-eut-73strings.azure-api.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 73 Strings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 73 Strings, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: 73 Strings
provider_slug: 73-strings
slug: 73-strings-domain-security
source_filename: 73-strings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.73strings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-accord-eut-73strings.developer.azure-api.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 21:42:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-accord-eut-73strings.azure-api.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 21:42:13 2027 GMT\n  hsts: null\ndomains:\n- domain: 73strings.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"letsencrypt.org,digicert.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: azure-api.net\n  dnssec: false\n  caa:\n\
  \  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/security/73-strings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- private-markets
- valuation
- portfolio-monitoring
- private-equity
- private-credit
- venture-capital
- alternative-assets
- financial-data
- data-extraction
- fintech
- asset-management
- azure-api-management
---
