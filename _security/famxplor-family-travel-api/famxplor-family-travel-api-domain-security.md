---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: famxplor.com
  spf: true
hosts:
- cert_expires: Sep  2 15:05:34 2026 GMT
  host: famxplor.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Famxplor Family Travel Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Famxplor Family Travel API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Famxplor Family Travel API
provider_slug: famxplor-family-travel-api
slug: famxplor-family-travel-api-domain-security
source_filename: famxplor-family-travel-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: famxplor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 15:05:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: famxplor.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/famxplor-family-travel-api/refs/heads/main/security/famxplor-family-travel-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Activities
- Family
- Travel
- AI
- MCP
---
