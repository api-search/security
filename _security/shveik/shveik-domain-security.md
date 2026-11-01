---
api_specs:
- filename: shveik-discovery-api-openapi.yml
  format: yaml
  label: shveik Discovery API
  slug: shveik-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shveik/openapi/shveik-discovery-api-openapi.yml
- filename: shveik-scraping-api-openapi.yml
  format: yaml
  label: shveik Scraping API
  slug: shveik-scraping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shveik/openapi/shveik-scraping-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shveik.dev
  spf: true
hosts:
- cert_expires: Jan 24 17:38:30 2027 GMT
  host: shveik.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 09:48:55 2026 GMT
  host: agdata.shveik.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 00:18:53 2027 GMT
  host: agmail.shveik.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Shveik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for shveik, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: shveik
provider_slug: shveik
slug: shveik-domain-security
source_filename: shveik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shveik.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 17:38:30 2027 GMT\n  hsts: false\n- host: agdata.shveik.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 09:48:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: agmail.shveik.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 00:18:53 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shveik.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/shveik/security/shveik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- x402
- Web Scraping
- Proxies
- Email
- VPS
- Escrow
- MCP
- Stablecoins
---
