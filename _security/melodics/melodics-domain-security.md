---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: melodics.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: melodics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Melodics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Melodics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Melodics
provider_slug: melodics
slug: melodics-domain-security
source_filename: melodics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: melodics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: melodics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/melodics/refs/heads/main/security/melodics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Music
- Music Education
- Education
- Learning
- MIDI
- EdTech
- Mobile App
---
