---
api_specs:
- filename: geekflare-openapi.json
  format: json
  label: Geekflare API
  slug: geekflare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geekflare/refs/heads/main/openapi/geekflare-openapi.json
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: geekflare.com
  spf: true
hosts:
- cert_expires: Nov 25 17:27:42 2026 GMT
  host: geekflare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 06:12:30 2026 GMT
  host: docs.geekflare.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 18:41:06 2026 GMT
  host: api.geekflare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Geekflare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geekflare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Geekflare
provider_slug: geekflare
slug: geekflare-domain-security
source_filename: geekflare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geekflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 17:27:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.geekflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 06:12:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.geekflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 18:41:06 2026 GMT\n  hsts: null\ndomains:\n- domain: geekflare.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geekflare/refs/heads/main/security/geekflare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Development
- Public APIs
- Web Scraping
- Search
- Screenshots
- DNS
- Website Monitoring
- Security Testing
- AI Agents
- MCP
---
