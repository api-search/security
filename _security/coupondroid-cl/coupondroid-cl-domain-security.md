---
api_specs:
- filename: coupondroid-cl-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid Chile A2a API
  slug: coupondroid-cl-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-a2a-api-openapi.yml
- filename: coupondroid-cl-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid Chile Auth.md API
  slug: coupondroid-cl-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-auth-md-api-openapi.yml
- filename: coupondroid-cl-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid Chile Llms.txt API
  slug: coupondroid-cl-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-llms-txt-api-openapi.yml
- filename: coupondroid-cl-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid Chile MCP API
  slug: coupondroid-cl-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-mcp-api-openapi.yml
- filename: coupondroid-cl-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid Chile .well Known API
  slug: coupondroid-cl-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-well-known-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: coupondroid.cl
  spf: true
hosts:
- cert_expires: Jan 15 08:15:35 2027 GMT
  host: coupondroid.cl
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coupondroid Chile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coupondroid Chile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Coupondroid Chile
provider_slug: coupondroid-cl
slug: coupondroid-cl-domain-security
source_filename: coupondroid-cl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coupondroid.cl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 08:15:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: coupondroid.cl\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-cl/security/coupondroid-cl-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Coupons
- Deals
- Discounts
- E-Commerce
- Affiliate Marketing
- Retail
- Chile
- MCP
---
