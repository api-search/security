---
api_specs:
- filename: sendoso-api-openapi.yml
  format: yaml
  label: Sendoso Sending Platform API
  slug: sendoso-sending-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/main/openapi/sendoso-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sendoso.com
  spf: true
hosts:
- cert_expires: Oct  2 05:17:03 2026 GMT
  host: sendoso.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 15:32:33 2026 GMT
  host: developer.sendoso.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: app.sendoso.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sendoso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sendoso, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sendoso
provider_slug: sendoso
slug: sendoso-domain-security
source_filename: sendoso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sendoso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:17:03 2026 GMT\n  hsts: false\n- host: developer.sendoso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 15:32:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.sendoso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sendoso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/security/sendoso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Corporate Gifting
- Direct Mail
- Sales Engagement
- Marketing Automation
- CRM Integration
---
