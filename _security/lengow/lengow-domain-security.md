---
api_specs:
- filename: lengow-authentication-api-openapi.yml
  format: yaml
  label: Lengow Authentication API
  slug: lengow-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lengow/refs/heads/main/openapi/lengow-authentication-api-openapi.yml
- filename: lengow-catalogues-api-openapi.yml
  format: yaml
  label: Lengow Catalogues API
  slug: lengow-catalogues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lengow/refs/heads/main/openapi/lengow-catalogues-api-openapi.yml
- filename: lengow-marketplaces-api-openapi.yml
  format: yaml
  label: Lengow Marketplaces API
  slug: lengow-marketplaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lengow/refs/heads/main/openapi/lengow-marketplaces-api-openapi.yml
- filename: lengow-rate-limits-api-openapi.yml
  format: yaml
  label: Lengow Rate limits API
  slug: lengow-rate-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lengow/refs/heads/main/openapi/lengow-rate-limits-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazonaws.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lengow.com
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "pki.goog"
  - 0 issue "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: lengow.io
  spf: false
hosts:
- cert_expires: Sep  5 02:27:09 2026 GMT
  host: www.lengow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:18:25 2026 GMT
  host: api.lengow.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lengow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lengow, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lengow
provider_slug: lengow
slug: lengow-domain-security
source_filename: lengow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lengow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 02:27:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lengow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:18:25 2026 GMT\n  hsts: null\ndomains:\n- domain: lengow.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lengow.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lengow/refs/heads/main/security/lengow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Software-as-a-Service
- E-Commerce
- Marketplaces
- Product Feeds
- Retail
- Advertising
- Order Management
- Price Intelligence
- France
---
