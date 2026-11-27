---
api_specs:
- filename: codeqr-io-analytics-api-openapi.yml
  format: yaml
  label: CodeQR Analytics API
  slug: codeqr-io-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-analytics-api-openapi.yml
- filename: codeqr-io-domains-api-openapi.yml
  format: yaml
  label: CodeQR Domains API
  slug: codeqr-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-domains-api-openapi.yml
- filename: codeqr-io-events-api-openapi.yml
  format: yaml
  label: CodeQR Events API
  slug: codeqr-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-events-api-openapi.yml
- filename: codeqr-io-folders-api-openapi.yml
  format: yaml
  label: CodeQR Folders API
  slug: codeqr-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-folders-api-openapi.yml
- filename: codeqr-io-links-api-openapi.yml
  format: yaml
  label: CodeQR Links API
  slug: codeqr-io-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-links-api-openapi.yml
- filename: codeqr-io-projects-api-openapi.yml
  format: yaml
  label: CodeQR Projects API
  slug: codeqr-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-projects-api-openapi.yml
- filename: codeqr-io-qr-codes-api-openapi.yml
  format: yaml
  label: CodeQR QR Codes API
  slug: codeqr-io-qr-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-qr-codes-api-openapi.yml
- filename: codeqr-io-tags-api-openapi.yml
  format: yaml
  label: CodeQR Tags API
  slug: codeqr-io-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-tags-api-openapi.yml
- filename: codeqr-io-track-api-openapi.yml
  format: yaml
  label: CodeQR Track API
  slug: codeqr-io-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-track-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: codeqr.io
  spf: true
hosts:
- cert_expires: Dec 30 09:06:43 2026 GMT
  host: codeqr.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CodeQR Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeQR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CodeQR
provider_slug: codeqr-io
slug: codeqr-io-domain-security
source_filename: codeqr-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codeqr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 09:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: codeqr.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/codeqr-io/security/codeqr-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- QR Codes
- Short Links
- URL Shorteners
- Link Management
- Analytics
- Marketing
- MCP
---
