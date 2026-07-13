---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: portlandgeneral.com
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: www.portlandgeneral.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.portlandgeneral.com
  https: false
- host: api.portlandgeneral.com
  https: false
kind: domain-security
layout: security
method: probed
name: Portland General Electric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portland General Electric, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Portland General Electric
provider_slug: portland-general-electric
slug: portland-general-electric-domain-security
source_filename: portland-general-electric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.portlandgeneral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.portlandgeneral.com\n  https: false\n- host: api.portlandgeneral.com\n  https: false\ndomains:\n- domain: portlandgeneral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portland-general-electric/refs/heads/main/security/portland-general-electric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Utilities
- Electric
- Energy
---
