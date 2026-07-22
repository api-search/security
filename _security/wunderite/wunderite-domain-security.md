---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wunderite.com
  spf: true
hosts:
- cert_expires: Oct  7 23:54:27 2026 GMT
  host: wunderite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:18:00 2026 GMT
  host: docs.wunderite.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:54:27 2026 GMT
  host: app.wunderite.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wunderite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wunderite, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wunderite
provider_slug: wunderite
slug: wunderite-domain-security
source_filename: wunderite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wunderite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:54:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.wunderite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:18:00 2026 GMT\n  hsts: false\n- host: app.wunderite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:54:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: wunderite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wunderite/refs/heads/main/security/wunderite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Insurtech
- ACORD Forms
- Risk Data
- Digital Signatures
- Insurance Applications
- Webhooks
---
