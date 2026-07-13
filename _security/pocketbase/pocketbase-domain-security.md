---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pocketbase.io
  spf: true
hosts:
- cert_expires: Sep 11 09:44:13 2026 GMT
  host: pocketbase.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: your-instance.pocketbase.io
  https: false
kind: domain-security
layout: security
method: probed
name: Pocketbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PocketBase, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PocketBase
provider_slug: pocketbase
slug: pocketbase-domain-security
source_filename: pocketbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pocketbase.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:44:13 2026 GMT\n  hsts: false\n- host: your-instance.pocketbase.io\n  https: false\ndomains:\n- domain: pocketbase.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pocketbase/refs/heads/main/security/pocketbase-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Backend-as-a-Service
- Open Source
- SQLite
- Realtime
- Authentication
- File Storage
- REST API
- Self-Hosted
- Go
---
