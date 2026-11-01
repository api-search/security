---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: runlane.run
  spf: false
hosts:
- cert_expires: Dec  6 00:19:48 2026 GMT
  host: runlane.run
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Runlane Run Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for runlane-run, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: runlane-run
provider_slug: runlane-run
slug: runlane-run-domain-security
source_filename: runlane-run-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runlane.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 00:19:48 2026 GMT\n  hsts: false\ndomains:\n- domain: runlane.run\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/runlane-run/security/runlane-run-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Productivity
- Task Management
- Solo Developers
- AI Integration
- Project Management
---
