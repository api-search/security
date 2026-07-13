---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Choozle Reporting API
  slug: choozle-reporting-api
  spec_type: OpenAPI
  url: https://app.choozle.com/apidoc/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: choozle.com
  spf: true
hosts:
- cert_expires: Oct  7 09:00:36 2026 GMT
  host: choozle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 19:01:06 2026 GMT
  host: help.choozle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 09:00:36 2026 GMT
  host: app.choozle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Choozle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Choozle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Choozle
provider_slug: choozle
slug: choozle-domain-security
source_filename: choozle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: choozle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:00:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.choozle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:01:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.choozle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:00:36 2026 GMT\n  hsts: false\ndomains:\n- domain: choozle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/choozle/refs/heads/main/security/choozle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Advertising
- Programmatic Advertising
- DSP
- Demand-Side Platform
- Campaign Management
- Audience Targeting
- Display Advertising
- Connected TV
- CTV
- Video Advertising
- Native Advertising
- DOOH
- Reporting
- Real-Time Bidding
- RTB
---
