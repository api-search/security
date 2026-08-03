---
api_specs:
- filename: pexa-exchange-api-swagger.json
  format: json
  label: PEXA Exchange API
  slug: pexa-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-exchange-api-swagger.json
- filename: pexa-standalone-discharge-experience-api-openapi.yaml
  format: yaml
  label: PEXA Standalone Discharge Experience API
  slug: pexa-standalone-discharge-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-standalone-discharge-experience-api-openapi.yaml
- filename: pexa-plus-marketplace-b2b-api-openapi.yaml
  format: yaml
  label: PEXA Plus Marketplace B2B API
  slug: pexa-plus-marketplace-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-plus-marketplace-b2b-api-openapi.yaml
- filename: pexa-notification-service-openapi.yaml
  format: yaml
  label: PEXA Notification Service [$]
  slug: pexa-notification-service-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-notification-service-openapi.yaml
- filename: pexa-projects-api-v4-openapi.yaml
  format: yaml
  label: PEXA Projects API
  slug: pexa-projects-api-v4-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-projects-api-v4-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pexa.com.au
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: www.pexa.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: developer.pexa.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.pexa.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pexa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PEXA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: PEXA
provider_slug: pexa
slug: pexa-domain-security
source_filename: pexa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pexa.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.pexa.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pexa.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pexa.com.au\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/security/pexa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Real Estate
- Australia
- Conveyancing
- Property Settlement
- Land Registry
- Title
- PropTech
- Mortgage
- Digital Signing
- Webhooks
---
