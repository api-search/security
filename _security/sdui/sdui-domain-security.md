---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sdui.de
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sdui.app
  spf: true
hosts:
- cert_expires: Oct 25 09:08:45 2026 GMT
  host: sdui.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 14:26:51 2026 GMT
  host: api.sdui.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sdui Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sdui, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sdui
provider_slug: sdui
slug: sdui-domain-security
source_filename: sdui-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sdui.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 09:08:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sdui.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 14:26:51 2026 GMT\n  hsts: null\ndomains:\n- domain: sdui.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sdui.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sdui/refs/heads/main/security/sdui-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Schools
- Communications
- Messaging
- Timetabling
- Grade Management
- Germany
- GDPR
---
