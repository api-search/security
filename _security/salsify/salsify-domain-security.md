---
api_specs:
- filename: salsify-api-settings-openapi.json
  format: json
  label: Salsify REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-api-settings-openapi.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "gandi.net"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: salsify.com
  spf: true
hosts:
- cert_expires: Oct 27 17:36:41 2026 GMT
  host: www.salsify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 04:12:00 2026 GMT
  host: developers.salsify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: app.salsify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salsify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salsify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Salsify
provider_slug: salsify
slug: salsify-domain-security
source_filename: salsify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.salsify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 17:36:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.salsify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:12:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.salsify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: salsify.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"gandi.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/security/salsify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Product Experience Management
- Product Information Management
- Digital Asset Management
- Commerce
- Retail
- Syndication
- Data Management
- SaaS
---
