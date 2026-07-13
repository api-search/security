---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: maximus.com
  spf: true
hosts:
- cert_expires: Sep  4 17:53:21 2026 GMT
  host: www.maximus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.maximus.com
  https: false
- host: api.maximus.com
  https: false
kind: domain-security
layout: security
method: probed
name: Maximus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maximus, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Maximus
provider_slug: maximus
slug: maximus-domain-security
source_filename: maximus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.maximus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 17:53:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.maximus.com\n  https: false\n- host: api.maximus.com\n  https: false\ndomains:\n- domain: maximus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maximus/refs/heads/main/security/maximus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government Services
- Health
- Technology
---
