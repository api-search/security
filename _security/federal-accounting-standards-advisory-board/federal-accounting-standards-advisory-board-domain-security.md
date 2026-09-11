---
api_specs:
- filename: federal-accounting-standards-advisory-board-wp-content-openapi.yml
  format: yaml
  label: FASAB Public Content API (WordPress REST)
  slug: federal-accounting-standards-advisory-board-wp-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-accounting-standards-advisory-board/refs/heads/main/openapi/federal-accounting-standards-advisory-board-wp-content-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fasab.gov
  spf: false
hosts:
- cert_expires: Oct 14 11:49:09 2026 GMT
  host: fasab.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Federal Accounting Standards Advisory Board Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Accounting Standards Advisory Board, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Federal Accounting Standards Advisory Board
provider_slug: federal-accounting-standards-advisory-board
slug: federal-accounting-standards-advisory-board-domain-security
source_filename: federal-accounting-standards-advisory-board-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fasab.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 11:49:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fasab.gov\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-accounting-standards-advisory-board/refs/heads/main/security/federal-accounting-standards-advisory-board-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Federal-Government
- Standards
- Financial-Reporting
- Government
- Regulations
- Content
- Publications
---
