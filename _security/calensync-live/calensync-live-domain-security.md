---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: calensync.live
  spf: true
hosts:
- cert_expires: Mar 23 23:59:59 2027 GMT
  host: calensync.live
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Calensync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calensync, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Calensync
provider_slug: calensync-live
slug: calensync-live-domain-security
source_filename: calensync-live-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calensync.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 23 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: calensync.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/calensync-live/security/calensync-live-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Calendar
- Sync
- Automation
- Software-as-a-Service
- Productivity
---
