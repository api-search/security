---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dataportal.se
  spf: true
hosts:
- cert_expires: Feb 25 14:00:14 2027 GMT
  host: www.dataportal.se
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Open Government Sweden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Sweden, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Government, Sweden
provider_slug: open-government-sweden
slug: open-government-sweden-domain-security
source_filename: open-government-sweden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dataportal.se\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 25 14:00:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dataportal.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-sweden/refs/heads/main/security/open-government-sweden-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Government
- Public APIs
---
