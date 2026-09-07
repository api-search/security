---
api_specs:
- filename: chocodata-openapi.json
  format: json
  label: Chocodata Scraper API
  slug: chocodata-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chocodata/refs/heads/main/openapi/chocodata-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: chocodata.com
  spf: true
hosts:
- cert_expires: Nov  1 01:47:31 2026 GMT
  host: chocodata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 03:56:52 2026 GMT
  host: api.chocodata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Chocodata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chocodata, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Chocodata
provider_slug: chocodata
slug: chocodata-domain-security
source_filename: chocodata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chocodata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 01:47:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.chocodata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 03:56:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chocodata.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chocodata/refs/heads/main/security/chocodata-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Web Scraping
- Data Extraction
- SERP
- E-Commerce Data
- social-media-data
- Proxy
- MCP
- agent-native
- structured-json
---
