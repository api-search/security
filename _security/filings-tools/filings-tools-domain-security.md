---
api_specs:
- filename: filings-tools-account-api-openapi.yml
  format: yaml
  label: filings.tools Account API
  slug: filings-tools-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filings-tools/openapi/filings-tools-account-api-openapi.yml
- filename: filings-tools-filings-api-openapi.yml
  format: yaml
  label: filings.tools Filings API
  slug: filings-tools-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filings-tools/openapi/filings-tools-filings-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: filings.tools
  spf: false
hosts:
- cert_expires: Dec 19 00:13:49 2026 GMT
  host: filings.tools
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: filings.tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for filings.tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: filings.tools
provider_slug: filings-tools
slug: filings-tools-domain-security
source_filename: filings-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: filings.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 00:13:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: filings.tools\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/filings-tools/security/filings-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- SEC Filings
- 10-K
- 10-Q
- 8-K
- Risk Factors
- Financial Documents
- Diff
- MCP
- Developer API
---
