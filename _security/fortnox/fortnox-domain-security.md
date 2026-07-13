---
api_specs:
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Invoices API
  slug: fortnox-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Customers API
  slug: fortnox-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Articles API
  slug: fortnox-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Orders API
  slug: fortnox-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Offers API
  slug: fortnox-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Bookkeeping API
  slug: fortnox-bookkeeping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Suppliers & Supplier Invoices API
  slug: fortnox-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Projects API
  slug: fortnox-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-asyncapi.yml
  format: yaml
  label: Fortnox Topics WebSocket API
  slug: fortnox-topics-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/asyncapi/fortnox-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "infocert.it"
  dmarc: true
  dmarc_policy: quarantine
  dmarc_subdomain_policy: quarantine
  dnssec: false
  domain: fortnox.se
  spf: true
  spf_record: v=spf1 ip4:168.245.43.210 ip4:168.245.29.251 ip4:149.72.127.118 include:_spf.google.com include:spfa.fortnox.se include:spfb.fortnox.se -all
hosts:
- cert_expires: Dec 25 12:49:54 2026 GMT
  cert_issuer: GlobalSign RSA OV SSL CA 2018
  host: api.fortnox.se
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  server: Fortnox
  tls_version: TLSv1.3
- cert_expires: Dec 25 12:49:54 2026 GMT
  cert_issuer: GlobalSign RSA OV SSL CA 2018
  host: ws.fortnox.se
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: WebSocket Topics endpoint (wss://ws.fortnox.se/topics-v1).
  server: Fortnox
  tls_version: TLSv1.3
- cert_expires: Dec 25 12:49:54 2026 GMT
  cert_issuer: GlobalSign RSA OV SSL CA 2018
  host: apps.fortnox.se
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: OAuth2 authorization/token host (oauth-v1/auth, oauth-v1/token).
  server: Fortnox
  tls_version: TLSv1.3
- cert_expires: Dec 25 12:49:54 2026 GMT
  cert_issuer: GlobalSign RSA OV SSL CA 2018
  host: www.fortnox.se
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  server: Fortnox
  tls_version: TLSv1.3
- cert_expires: Dec 25 12:49:54 2026 GMT
  cert_issuer: GlobalSign RSA OV SSL CA 2018
  host: developer.fortnox.se
  https: true
  redirect: https://www.fortnox.se/developer
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fortnox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortnox, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fortnox
provider_slug: fortnox
slug: fortnox-domain-security
source_filename: fortnox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + API/WebSocket hosts\nprovider: Fortnox\nproviderId: fortnox\nhosts:\n- host: api.fortnox.se\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GlobalSign RSA OV SSL CA 2018\n  cert_expires: Dec 25 12:49:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: Fortnox\n- host: ws.fortnox.se\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GlobalSign RSA OV SSL CA 2018\n  cert_expires: Dec 25 12:49:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: Fortnox\n  note: WebSocket Topics endpoint (wss://ws.fortnox.se/topics-v1).\n- host: apps.fortnox.se\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GlobalSign RSA OV SSL CA 2018\n  cert_expires: Dec 25 12:49:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: Fortnox\n  note: OAuth2 authorization/token\
  \ host (oauth-v1/auth, oauth-v1/token).\n- host: www.fortnox.se\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GlobalSign RSA OV SSL CA 2018\n  cert_expires: Dec 25 12:49:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: Fortnox\n- host: developer.fortnox.se\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GlobalSign RSA OV SSL CA 2018\n  cert_expires: Dec 25 12:49:54 2026 GMT\n  redirect: https://www.fortnox.se/developer\ndomains:\n- domain: fortnox.se\n  dnssec: false\n  spf: true\n  spf_record: 'v=spf1 ip4:168.245.43.210 ip4:168.245.29.251 ip4:149.72.127.118 include:_spf.google.com include:spfa.fortnox.se include:spfb.fortnox.se -all'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_subdomain_policy: quarantine\n  caa:\n  - '0 issue \"globalsign.com\"'\n  - '0 issue \"digicert.com; cansignhttpexchanges=yes\"'\n  - '0 issue \"letsencrypt.org\"'\n  - '0 issue \"pki.goog; cansignhttpexchanges=yes\"'\n  - '0 issue \"ssl.com\"\
  '\n  - '0 issue \"comodoca.com\"'\n  - '0 issue \"infocert.it\"'\nnotes: >-\n  All Fortnox API, WebSocket, OAuth, and web hosts serve TLS 1.3 with GlobalSign\n  OV certificates and enforce HSTS (max-age 31536000, includeSubdomains). The\n  fortnox.se apex publishes SPF (-all), DMARC (p=quarantine), and a restrictive\n  CAA allow-list. DNSSEC was not observed on the apex at probe time.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/security/fortnox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- ERP
- Invoicing
- Bookkeeping
- Sweden
- Nordics
- Finance
- Vouchers
- Customers
- SaaS
---
