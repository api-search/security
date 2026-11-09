---
api_specs:
- filename: 4dayweek-io-4dayweek-io-public-api-api-openapi.yml
  format: yaml
  label: 4dayweek-io 4dayweek.io Public API
  slug: 4dayweek-io-4dayweek-io-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4dayweek-io/openapi/4dayweek-io-4dayweek-io-public-api-api-openapi.yml
- filename: 4dayweek-io-jobs-api-openapi.yml
  format: yaml
  label: 4dayweek-io Jobs API
  slug: 4dayweek-io-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4dayweek-io/openapi/4dayweek-io-jobs-api-openapi.yml
- filename: 4dayweek-io-mcp-api-openapi.yml
  format: yaml
  label: 4dayweek-io MCP API
  slug: 4dayweek-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4dayweek-io/openapi/4dayweek-io-mcp-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 4dayweek.io
  spf: true
hosts:
- cert_expires: Dec 12 23:01:02 2026 GMT
  host: 4dayweek.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 4Dayweek Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4dayweek-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 4dayweek-io
provider_slug: 4dayweek-io
slug: 4dayweek-io-domain-security
source_filename: 4dayweek-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 4dayweek.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:01:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 4dayweek.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/4dayweek-io/security/4dayweek-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Remote Jobs
- Flexible Schedule
- Work-Life Balance
- Recruiting
---
