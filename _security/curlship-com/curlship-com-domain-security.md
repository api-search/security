---
api_specs:
- filename: curlship-com-badge-api-openapi.yml
  format: yaml
  label: CurlShip Badge API
  slug: curlship-com-badge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curlship-com/openapi/curlship-com-badge-api-openapi.yml
- filename: curlship-com-billing-api-openapi.yml
  format: yaml
  label: CurlShip Billing API
  slug: curlship-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curlship-com/openapi/curlship-com-billing-api-openapi.yml
- filename: curlship-com-edits-api-openapi.yml
  format: yaml
  label: CurlShip Edits API
  slug: curlship-com-edits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curlship-com/openapi/curlship-com-edits-api-openapi.yml
- filename: curlship-com-listings-api-openapi.yml
  format: yaml
  label: CurlShip Listings API
  slug: curlship-com-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curlship-com/openapi/curlship-com-listings-api-openapi.yml
- filename: curlship-com-stats-api-openapi.yml
  format: yaml
  label: CurlShip Stats API
  slug: curlship-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curlship-com/openapi/curlship-com-stats-api-openapi.yml
- filename: curlship-com-x402-api-openapi.yml
  format: yaml
  label: CurlShip X402 API
  slug: curlship-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curlship-com/openapi/curlship-com-x402-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: curlship.com
  spf: true
hosts:
- cert_expires: Jan  2 20:44:07 2027 GMT
  host: curlship.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CurlShip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CurlShip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CurlShip
provider_slug: curlship-com
slug: curlship-com-domain-security
source_filename: curlship-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curlship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 20:44:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: curlship.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/curlship-com/security/curlship-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Directory
- Product Listings
- Developer Tools
- MCP
- AI Agents
- REST API
- Launch Platform
---
