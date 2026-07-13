---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: forismatic.com
  spf: false
hosts:
- cert_expires: Aug 30 12:37:51 2026 GMT
  host: forismatic.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forismatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forismatic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Forismatic
provider_slug: forismatic
slug: forismatic-domain-security
source_filename: forismatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forismatic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 12:37:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: forismatic.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forismatic/refs/heads/main/security/forismatic-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Personality
- Public APIs
---
