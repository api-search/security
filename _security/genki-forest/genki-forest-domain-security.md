---
api_specs:
- filename: genki-forest-open-platform-swagger.json
  format: json
  label: Genki Forest Open Platform — Distributor & Receivables Management
  slug: genki-forest-open-platform-distributor-receivables-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genki-forest/refs/heads/main/openapi/genki-forest-open-platform-swagger.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yuanqisenlin.com
  spf: true
hosts:
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: www.yuanqisenlin.com
  hsts: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: open.yuanqisenlin.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15724800
  https: true
  note: 'HSTS is served on this host but the automated probe recorded null because GET / returns 405 Method Not Allowed (the gateway root accepts POST only). Header observed verbatim on that 405 response: Strict-Transport-Security: max-age=15724800; includeSubDomains.'
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Genki Forest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genki Forest, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Genki Forest
provider_slug: genki-forest
slug: genki-forest-domain-security
source_filename: genki-forest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yuanqisenlin.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\n- host: open.yuanqisenlin.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n  hsts_include_subdomains: true\n  note: >-\n    HSTS is served on this host but the automated probe recorded null because GET / returns\n    405 Method Not Allowed (the gateway root accepts POST only). Header observed verbatim on\n    that 405 response: Strict-Transport-Security: max-age=15724800; includeSubDomains.\ndomains:\n- domain: yuanqisenlin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genki-forest/refs/heads/main/security/genki-forest-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Beverages
- Food and Beverage
- Consumer Packaged Goods
- Manufacturing
- Distribution
- Retail
- China
---
