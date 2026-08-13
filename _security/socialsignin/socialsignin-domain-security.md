---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: socialsignin.com
  spf: true
- caa:
  - 128 issue "godaddy.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: socialsign.in
  note: SPF includes _spf.google.com, mail.zendesk.com, sendgrid.net, spf.mandrillapp.com and a HubSpot sending domain. DMARC rua reports to EasyDMARC. Probed 2026-08-12.
  spf: true
hosts:
- cert_expires: Oct 14 20:11:08 2026 GMT
  host: socialsignin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 21 16:22:47 2026 GMT
  host: socialsign.in
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 21 16:22:47 2026 GMT
  host: c.socialsign.in
  hsts: false
  hsts_max_age: null
  https: true
  note: Customer console host. Sends X-Frame-Options sameorigin, X-Content-Type-Options nosniff and X-XSS-Protection, but no Strict-Transport-Security.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Socialsignin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SocialSign.in, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SocialSign.in
provider_slug: socialsignin
slug: socialsignin-domain-security
source_filename: socialsignin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: socialsignin.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 14 20:11:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: socialsign.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 16:22:47 2026 GMT\n  hsts: false\n  hsts_max_age: null\n- host: c.socialsign.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 16:22:47 2026 GMT\n  hsts: false\n  hsts_max_age: null\n  note: >-\n    Customer console host. Sends X-Frame-Options sameorigin, X-Content-Type-Options\n    nosniff and X-XSS-Protection, but no Strict-Transport-Security.\ndomains:\n- domain: socialsignin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: socialsign.in\n  dnssec: false\n  caa:\n  - 128 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: >-\n    SPF includes _spf.google.com,\
  \ mail.zendesk.com, sendgrid.net,\n    spf.mandrillapp.com and a HubSpot sending domain. DMARC rua reports to\n    EasyDMARC. Probed 2026-08-12.\nx-probe-note: >-\n  socialsign.in and c.socialsign.in were probed by hand on 2026-08-12 and merged\n  into this file; probe-domain-security.py only saw socialsignin.com because the\n  other hosts were not yet named as an apis.yml host at run time.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socialsignin/refs/heads/main/security/socialsignin-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Guest WiFi
- WiFi Marketing
- Captive Portal
- Customer Data Platform
- Location Analytics
- Retail Media
- Marketing
---
