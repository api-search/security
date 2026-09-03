---
api_specs:
- filename: tempmailgrab-openapi.json
  format: json
  label: TempMailGrab REST API
  slug: tempmailgrab-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tempmailgrab/refs/heads/main/openapi/tempmailgrab-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tempmailgrab.com
  spf: true
hosts:
- cert_expires: Nov 12 23:44:16 2026 GMT
  host: tempmailgrab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tempmailgrab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TempMailGrab API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TempMailGrab API
provider_slug: tempmailgrab
slug: tempmailgrab-domain-security
source_filename: tempmailgrab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tempmailgrab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:44:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tempmailgrab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tempmailgrab/refs/heads/main/security/tempmailgrab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- email
- temporary-email
- disposable-email
- otp
- webhooks
- qa
- testing
- playwright
- cypress
- developer-tools
- email-testing
- ci
---
