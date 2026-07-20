---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trychert.com
  spf: true
hosts:
- cert_expires: Sep 27 12:37:22 2026 GMT
  host: docs.trychert.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 21:18:25 2026 GMT
  host: console.trychert.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chert, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chert
provider_slug: chert
slug: chert-domain-security
source_filename: chert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.trychert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:37:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: console.trychert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 21:18:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trychert.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chert/refs/heads/main/security/chert-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Messaging
- iMessage
- Communications
- Conversational
- Webhooks
- CRM Integration
- API
---
