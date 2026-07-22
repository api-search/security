---
api_specs:
- filename: unrivaled-basketball-openapi.yml
  format: yaml
  label: Unrivaled API
  slug: unrivaled-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrivaled-basketball/refs/heads/main/openapi/unrivaled-basketball-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unrivaled.basketball
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sportradar.com
  spf: true
hosts:
- cert_expires: Sep  7 21:24:44 2026 GMT
  host: www.unrivaled.basketball
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 01:36:45 2026 GMT
  host: developer.sportradar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: api.sportradar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unrivaled Basketball Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unrivaled Basketball, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unrivaled Basketball
provider_slug: unrivaled-basketball
slug: unrivaled-basketball-domain-security
source_filename: unrivaled-basketball-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unrivaled.basketball\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:24:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.sportradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 01:36:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sportradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: unrivaled.basketball\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sportradar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unrivaled-basketball/refs/heads/main/security/unrivaled-basketball-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Basketball
- Sports
- Womens Sports
- Sports Data
- Media
- League
---
