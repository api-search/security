---
api_specs:
- filename: klook-octo-openapi-original.json
  format: json
  label: Klook Open API (OCTO)
  slug: klook-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klook/refs/heads/main/openapi/klook-octo-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: klook.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitbook.io
  spf: true
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: www.klook.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 19:03:12 2026 GMT
  host: klook.gitbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klook, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Klook
provider_slug: klook
slug: klook-domain-security
source_filename: klook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.klook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: null\n- host: klook.gitbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:03:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: klook.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gitbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klook/refs/heads/main/security/klook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplaces
- Travel
- Tours and Activities
- Booking
- Experiences
- Distribution
- OCTO
- Hospitality
---
