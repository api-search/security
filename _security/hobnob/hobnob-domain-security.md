---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hobnob.app
  spf: false
hosts:
- cert_expires: Oct 15 14:55:02 2026 GMT
  host: hobnob.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hobnob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hobnob, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Hobnob
provider_slug: hobnob
slug: hobnob-domain-security
source_filename: hobnob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hobnob.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 14:55:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: hobnob.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hobnob/refs/heads/main/security/hobnob-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Events
- Invitations
- RSVP
- Ticketing
- Community
- Social
- Consumer
- Mobile App
---
