---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sync-api.com
  spf: true
hosts:
- cert_expires: Aug 23 22:26:45 2026 GMT
  host: sync-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.sync-api.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sync Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sync API, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sync API
provider_slug: sync-api
slug: sync-api-domain-security
source_filename: sync-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sync-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 22:26:45 2026 GMT\n  hsts: false\n- host: api.sync-api.com\n  https: false\ndomains:\n- domain: sync-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sync-api/refs/heads/main/security/sync-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- Digital Marketing
- In-App Advertising
- Mobile
- Programmatic
- Real-Time Bidding
- User Acquisition
---
