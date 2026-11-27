---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hearth.rsvp
  spf: true
hosts:
- cert_expires: Jan 25 14:16:22 2027 GMT
  host: hearth.rsvp
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hearth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hearth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hearth
provider_slug: hearth-rsvp
slug: hearth-rsvp-domain-security
source_filename: hearth-rsvp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hearth.rsvp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 14:16:22 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hearth.rsvp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hearth-rsvp/security/hearth-rsvp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Invitation
- Event
- RSVP
- Web App
---
