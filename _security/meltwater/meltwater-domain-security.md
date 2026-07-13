---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Meltwater API
  slug: meltwater-api
  spec_type: OpenAPI
  url: https://developer.meltwater.com/api-reference/api-reference-overview/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meltwater.com
  spf: true
hosts:
- cert_expires: Aug 30 04:31:11 2026 GMT
  host: www.meltwater.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: developer.meltwater.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: api.meltwater.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Meltwater Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meltwater, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Meltwater
provider_slug: meltwater
slug: meltwater-domain-security
source_filename: meltwater-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meltwater.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 04:31:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.meltwater.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\n- host: api.meltwater.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: meltwater.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/security/meltwater-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Media Monitoring
- Social Listening
- PR Analytics
- Brand Intelligence
- News API
- Social Analytics
- Media Intelligence
---
