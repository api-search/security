---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: resulticks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: resu.io
  spf: true
hosts:
- cert_expires: Nov  6 09:55:20 2026 GMT
  host: www.resulticks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 09:55:20 2026 GMT
  host: gud.resulticks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: apis.resu.io
  https: false
kind: domain-security
layout: security
method: probed
name: Resulticks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resulticks, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Resulticks
provider_slug: resulticks
slug: resulticks-domain-security
source_filename: resulticks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.resulticks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 09:55:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gud.resulticks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 09:55:20 2026 GMT\n  hsts: false\n- host: apis.resu.io\n  https: false\ndomains:\n- domain: resulticks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: resu.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resulticks/refs/heads/main/security/resulticks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Marketing Automation
- Omnichannel
- Customer Engagement
- Customer Data Platform
- MarTech
- Campaign Management
- Audience
- Analytics
- Messaging
- SMS
- Email
- Push Notifications
- WhatsApp
---
