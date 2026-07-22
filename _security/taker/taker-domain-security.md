---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: taker.io
  spf: true
  spf_record: v=spf1 include:transmail.net include:spf.protection.outlook.com include:zcsend.net ~all
hosts:
- host: production.go.taker.io
  hsts: false
  https: true
  server: nginx
- host: sandbox.go.taker.io
  hsts: false
  https: true
  server: nginx
- host: api.help.taker.io
  hsts: false
  https: true
  server: nginx/1.18.0 (Ubuntu)
- cert_not_after: '2026-09-18'
  host: taker.io
  hsts: false
  https: true
  server: nginx
kind: domain-security
layout: security
method: probed
name: Taker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taker, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Taker
provider_slug: taker
slug: taker-domain-security
source_filename: taker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live probe (curl HEAD + dig)\nhosts:\n  - {host: production.go.taker.io, https: true, server: nginx, hsts: false}\n  - {host: sandbox.go.taker.io, https: true, server: nginx, hsts: false}\n  - {host: api.help.taker.io, https: true, server: \"nginx/1.18.0 (Ubuntu)\", hsts: false}\n  - {host: taker.io, https: true, server: nginx, hsts: false, cert_not_after: \"2026-09-18\"}\ndomains:\n  - domain: taker.io\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: \"v=spf1 include:transmail.net include:spf.protection.outlook.com include:zcsend.net ~all\"\n    dmarc: false\n    dmarc_policy: null\nnotes: >-\n  All probed hosts serve HTTPS but none set an HSTS response header. The\n  taker.io registrable domain publishes an SPF record (Zoho TransMail,\n  Microsoft 365/Outlook, Zoho ZeptoMail) with a soft-fail (~all) policy but\n  has no DMARC record, no CAA records, and no DNSSEC. Absence of these records\n  is recorded as observed\
  \ data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taker/refs/heads/main/security/taker-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Restaurant Technology
- Online Ordering
- Food Delivery
- Delivery Integration
- Webhooks
- Saudi Arabia
- MENA
---
