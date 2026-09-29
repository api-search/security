---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bloomboard.com
  spf: true
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: bloomboard.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bloomboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bloomboard
provider_slug: bloomboard
slug: bloomboard-domain-security
source_filename: bloomboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bloomboard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bloomboard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomboard/refs/heads/main/security/bloomboard-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Education
- Talent Development
- K-12
- Higher Education
- Workforce
---
