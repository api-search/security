---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: matw.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.matw.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.matw.com
  https: false
- host: api.matw.com
  https: false
kind: domain-security
layout: security
method: probed
name: Matthews International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matthews International, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Matthews International
provider_slug: matthews-international
slug: matthews-international-domain-security
source_filename: matthews-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.matw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.matw.com\n  https: false\n- host: api.matw.com\n  https: false\ndomains:\n- domain: matw.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matthews-international/refs/heads/main/security/matthews-international-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Memorialization
- Branding
- Industrial
---
