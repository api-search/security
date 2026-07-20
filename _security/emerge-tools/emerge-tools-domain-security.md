---
api_specs:
- filename: emerge-tools-openapi.json
  format: json
  label: Emerge API
  slug: emerge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: emergetools.com
  spf: true
hosts:
- cert_expires: Oct 11 14:01:27 2026 GMT
  host: emergetools.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 14:01:27 2026 GMT
  host: api.emergetools.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emerge Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emerge Tools, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Emerge Tools
provider_slug: emerge-tools
slug: emerge-tools-domain-security
source_filename: emerge-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emergetools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:01:27 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.emergetools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:01:27 2026 GMT\n  hsts: null\ndomains:\n- domain: emergetools.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/security/emerge-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- B2B
- Mobile
- Developer Tools
- App Performance
- Testing
- iOS
- Android
- DevOps
---
