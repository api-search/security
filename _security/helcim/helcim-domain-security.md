---
api_specs:
- filename: helcim-ach-payment-api-openapi.yml
  format: yaml
  label: Helcim ACH Payment API
  slug: helcim-ach-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-ach-payment-api-openapi.yml
- filename: helcim-card-batch-api-openapi.yml
  format: yaml
  label: Helcim Card Batch API
  slug: helcim-card-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-card-batch-api-openapi.yml
- filename: helcim-card-terminal-api-openapi.yml
  format: yaml
  label: Helcim Card Terminal API
  slug: helcim-card-terminal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-card-terminal-api-openapi.yml
- filename: helcim-card-transaction-api-openapi.yml
  format: yaml
  label: Helcim Card Transaction API
  slug: helcim-card-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-card-transaction-api-openapi.yml
- filename: helcim-customer-api-openapi.yml
  format: yaml
  label: Helcim Customer API
  slug: helcim-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-customer-api-openapi.yml
- filename: helcim-device-api-openapi.yml
  format: yaml
  label: Helcim Device API
  slug: helcim-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-device-api-openapi.yml
- filename: helcim-general-api-openapi.yml
  format: yaml
  label: Helcim General API
  slug: helcim-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-general-api-openapi.yml
- filename: helcim-invoice-api-openapi.yml
  format: yaml
  label: Helcim Invoice API
  slug: helcim-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-invoice-api-openapi.yml
- filename: helcim-payment-api-openapi.yml
  format: yaml
  label: Helcim Payment API
  slug: helcim-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-payment-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: helcim.com
  spf: true
hosts:
- cert_expires: Oct  7 03:46:33 2026 GMT
  host: www.helcim.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 15:59:33 2026 GMT
  host: devdocs.helcim.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:46:33 2026 GMT
  host: api.helcim.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helcim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helcim, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Helcim
provider_slug: helcim
slug: helcim-domain-security
source_filename: helcim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helcim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:46:33 2026 GMT\n  hsts: null\n- host: devdocs.helcim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:59:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.helcim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:46:33 2026 GMT\n  hsts: null\ndomains:\n- domain: helcim.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/security/helcim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Canada
- Payment Gateway
- Payment Processing
- Acquiring
- Merchant Services
- ACH
- Invoicing
- Card Terminal
- Small Business
---
