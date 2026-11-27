---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: coachsync.io
  spf: true
hosts:
- cert_expires: Jan 20 18:23:25 2027 GMT
  host: coachsync.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CoachSync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoachSync, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CoachSync
provider_slug: coachsync-io
slug: coachsync-io-domain-security
source_filename: coachsync-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coachsync.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 18:23:25 2027 GMT\n  hsts: false\ndomains:\n- domain: coachsync.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/coachsync-io/security/coachsync-io-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Coaching
- Fitness
- Strength Training
- Workout Programming
- Software-as-a-Service
- MCP
---
