---
api_specs:
- filename: steel-dev-openapi.yml
  format: yaml
  label: Steel Sessions API
  slug: steel-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steel-dev/refs/heads/main/openapi/steel-dev-openapi.yml
- filename: steel-dev-openapi.yml
  format: yaml
  label: Steel Scrape API
  slug: steel-scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steel-dev/refs/heads/main/openapi/steel-dev-openapi.yml
- filename: steel-dev-openapi.yml
  format: yaml
  label: Steel Screenshot & PDF API
  slug: steel-screenshot-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steel-dev/refs/heads/main/openapi/steel-dev-openapi.yml
- filename: steel-dev-openapi.yml
  format: yaml
  label: Steel CDP / Browser Connect API
  slug: steel-browser-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steel-dev/refs/heads/main/openapi/steel-dev-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: steel.dev
  spf: false
hosts:
- cert_expires: Sep 18 13:34:45 2026 GMT
  host: steel.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 19:05:18 2026 GMT
  host: docs.steel.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 22:22:48 2026 GMT
  host: api.steel.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Steel Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Steel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Steel
provider_slug: steel-dev
slug: steel-dev-domain-security
source_filename: steel-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: steel.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:34:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.steel.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:05:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.steel.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:22:48 2026 GMT\n  hsts: false\ndomains:\n- domain: steel.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steel-dev/refs/heads/main/security/steel-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Browser
- Web Automation
- Scraping
- AI Agents
- Open Source
---
