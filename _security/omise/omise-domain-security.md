---
api_specs:
- filename: omise-openapi.yml
  format: yaml
  label: Omise Charges API
  slug: omise-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Tokens API
  slug: omise-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Sources API
  slug: omise-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Customers API
  slug: omise-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Refunds API
  slug: omise-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Disputes API
  slug: omise-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Transfers API
  slug: omise-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Recipients API
  slug: omise-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Schedules API
  slug: omise-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Links API
  slug: omise-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Events API
  slug: omise-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Account and Balance API
  slug: omise-account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "geotrust.com"
  - 0 issue "visa.com"
  - 0 issuewild "thawte.com"
  - 0 iodef "mailto:security@omise.co"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: omise.co
  spf: true
  spf_record: v=spf1 include:mailgun.org include:_spf.google.com ~all
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  cert_issuer: Thawte TLS RSA CA G1 (DigiCert)
  cert_not_before: Sep 18 00:00:00 2025 GMT
  host: api.omise.co
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  note: Returns HTTP 401 without credentials (HTTP Basic secret key required).
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  cert_issuer: Thawte TLS RSA CA G1 (DigiCert)
  cert_not_before: Sep 18 00:00:00 2025 GMT
  host: vault.omise.co
  hsts: false
  https: true
  note: PCI-scoped tokenization host; public key required. HSTS header not observed on probe.
  tls_version: TLSv1.3
- cert_expires: Aug 17 15:37:16 2026 GMT
  cert_issuer: Google Trust Services WE1
  cert_not_before: May 19 14:37:17 2026 GMT
  host: www.omise.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omise, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Omise
provider_slug: omise
slug: omise-domain-security
source_filename: omise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.omise.co\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Thawte TLS RSA CA G1 (DigiCert)\n  cert_not_before: Sep 18 00:00:00 2025 GMT\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  note: Returns HTTP 401 without credentials (HTTP Basic secret key required).\n- host: vault.omise.co\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Thawte TLS RSA CA G1 (DigiCert)\n  cert_not_before: Sep 18 00:00:00 2025 GMT\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: false\n  note: PCI-scoped tokenization host; public key required. HSTS header not observed on probe.\n- host: www.omise.co\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services WE1\n  cert_not_before: May 19 14:37:17 2026 GMT\n  cert_expires: Aug 17 15:37:16 2026 GMT\n  hsts: true\n  hsts_max_age:\
  \ 31536000\n  server: cloudflare\ndomains:\n- domain: omise.co\n  dnssec: false\n  caa:\n  - '0 issue \"digicert.com\"'\n  - '0 issue \"amazon.com\"'\n  - '0 issue \"amazonaws.com\"'\n  - '0 issue \"amazontrust.com\"'\n  - '0 issue \"letsencrypt.org\"'\n  - '0 issue \"pki.goog; cansignhttpexchanges=yes\"'\n  - '0 issue \"sectigo.com\"'\n  - '0 issue \"geotrust.com\"'\n  - '0 issue \"visa.com\"'\n  - '0 issuewild \"thawte.com\"'\n  - '0 iodef \"mailto:security@omise.co\"'\n  spf: true\n  spf_record: v=spf1 include:mailgun.org include:_spf.google.com ~all\n  dmarc: true\n  dmarc_policy: reject\nnotes: >-\n  Probed 2026-07-12. api.omise.co and vault.omise.co are the two API hosts. The\n  core API host enforces HTTPS with a two-year HSTS max-age and includeSubDomains,\n  and rejects unauthenticated requests with 401. CAA records restrict issuance to\n  a defined set of CAs and publish a security iodef contact (security@omise.co).\n  DMARC is set to p=reject. DNSSEC was not observed on omise.co\
  \ at probe time.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/security/omise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Thailand
- Southeast Asia
- Charges
- Tokens
- Sources
- PromptPay
- Cards
- Fintech
---
