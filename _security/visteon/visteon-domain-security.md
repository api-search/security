---
api_specs:
- filename: visteon-phoenix-openapi.yml
  format: yaml
  label: Visteon Phoenix API
  slug: phoenix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visteon/refs/heads/main/openapi/visteon-phoenix-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: visteon.com
  spf: true
hosts:
- cert_expires: Oct  9 14:07:29 2026 GMT
  host: www.visteon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.visteon.com
  https: false
kind: domain-security
layout: security
method: probed
name: Visteon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Visteon, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Visteon
provider_slug: visteon
slug: visteon-domain-security
source_filename: visteon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.visteon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:07:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.visteon.com\n  https: false\ndomains:\n- domain: visteon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visteon/refs/heads/main/security/visteon-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Automotive
- Connected Car
- Infotainment
- IoT
- Fortune 500
---
