---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: tbo.com
  spf: true
hosts:
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: tbo.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tbo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TBO.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: TBO.com
provider_slug: tbo
slug: tbo-domain-security
source_filename: tbo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tbo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: tbo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tbo/refs/heads/main/security/tbo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC
tags:
- Travel
- Distribution
- API
- B2B
- Platform
---
