---
api_specs:
- filename: standard-metrics-main-openapi.json
  format: json
  label: Standard Metrics API
  slug: standard-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-main-openapi.json
- filename: standard-metrics-investment-data-openapi.json
  format: json
  label: Standard Metrics Investment Data API
  slug: standard-metrics-investment-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-investment-data-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  - 0 issue "cloudflare.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: standardmetrics.io
  spf: true
hosts:
- cert_expires: Sep 27 21:44:22 2026 GMT
  host: standardmetrics.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 15:20:52 2026 GMT
  host: api.standardmetrics.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 15:20:52 2026 GMT
  host: app.standardmetrics.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Standard Metrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Standard Metrics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Standard Metrics
provider_slug: standard-metrics
slug: standard-metrics-domain-security
source_filename: standard-metrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: standardmetrics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:44:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.standardmetrics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 15:20:52 2026 GMT\n  hsts: null\n- host: app.standardmetrics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 15:20:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: standardmetrics.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/security/standard-metrics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Venture Capital
- Private Equity
- Portfolio Management
- Financial Data
- Investment Data
- Cap Table
- Metrics
- Reporting
- MCP
---
