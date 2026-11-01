---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: syncsmart.io
  spf: true
hosts:
- cert_expires: Dec  2 18:50:01 2026 GMT
  host: syncsmart.io
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Syncsmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SyncSmart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SyncSmart
provider_slug: syncsmart
slug: syncsmart-domain-security
source_filename: syncsmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syncsmart.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 18:50:01 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: syncsmart.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/syncsmart/security/syncsmart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Integration
- HubSpot
- Marketing
- Sales
- Automation
---
