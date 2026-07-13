---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: powersync.com
  spf: true
hosts:
- cert_expires: Oct  6 16:28:26 2026 GMT
  host: powersync.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:26:36 2026 GMT
  host: docs.powersync.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Powersync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PowerSync, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PowerSync
provider_slug: powersync
slug: powersync-domain-security
source_filename: powersync-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: powersync.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:28:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.powersync.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:26:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: powersync.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powersync/refs/heads/main/security/powersync-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Database
- Sync
- Offline-First
- SQLite
- Local-First
- Real-Time
---
