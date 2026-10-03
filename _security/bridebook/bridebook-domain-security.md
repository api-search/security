---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bridebook.com
  spf: true
hosts:
- cert_expires: Dec  8 14:01:29 2026 GMT
  host: bridebook.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bridebook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bridebook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bridebook
provider_slug: bridebook
slug: bridebook-domain-security
source_filename: bridebook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bridebook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 14:01:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bridebook.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridebook/refs/heads/main/security/bridebook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Wedding Planning
- Online Planner
- Free App
- Couples
---
