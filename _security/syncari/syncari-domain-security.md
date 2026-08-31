---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: syncari.com
  spf: true
hosts:
- cert_expires: Oct  2 19:35:00 2026 GMT
  host: syncari.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:46:28 2026 GMT
  host: support.syncari.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 11:19:31 2026 GMT
  host: api.syncari.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Syncari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syncari, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Syncari
provider_slug: syncari
slug: syncari-domain-security
source_filename: syncari-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syncari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:35:00 2026 GMT\n  hsts: false\n- host: support.syncari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:46:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.syncari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 11:19:31 2026 GMT\n  hsts: null\ndomains:\n- domain: syncari.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syncari/refs/heads/main/security/syncari-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Master Data Management
- Data Unification
- Data Integration
- iPaaS
- Data Quality
- Data Governance
- Embedded Integration
- MCP
- agent-native
- RevOps
- Data Synchronization
---
