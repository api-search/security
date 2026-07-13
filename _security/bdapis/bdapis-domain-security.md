---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bdapis.com
  spf: false
hosts:
- cert_expires: Oct  2 13:42:57 2026 GMT
  host: bdapis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bdapis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BdAPIs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BdAPIs
provider_slug: bdapis
slug: bdapis-domain-security
source_filename: bdapis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bdapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:42:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bdapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bdapis/refs/heads/main/security/bdapis-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Geocoding
- Public APIs
---
