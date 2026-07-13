---
api_specs:
- filename: wati-openapi.yml
  format: yaml
  label: WATI WhatsApp Business API
  slug: whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wati/refs/heads/main/openapi/wati-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: wati.io
  spf: true
hosts:
- cert_expires: Aug 26 03:08:59 2026 GMT
  host: www.wati.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 09:37:39 2026 GMT
  host: docs.wati.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 22:20:23 2026 GMT
  host: live-mt-server.wati.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wati Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WATI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: WATI
provider_slug: wati
slug: wati-domain-security
source_filename: wati-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wati.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 03:08:59 2026 GMT\n  hsts: false\n- host: docs.wati.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:37:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: live-mt-server.wati.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:20:23 2026 GMT\n  hsts: false\ndomains:\n- domain: wati.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wati/refs/heads/main/security/wati-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- WhatsApp
- Messaging
- Customer Engagement
- Chatbot
- Business Communication
- CRM
---
