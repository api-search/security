---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meetmarigold.com
  spf: true
hosts:
- cert_expires: Sep 18 23:37:08 2026 GMT
  host: meetmarigold.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 20:59:48 2026 GMT
  host: sdkdevelopers.meetmarigold.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carnival Mobile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carnival Mobile *, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Carnival Mobile *
provider_slug: carnival-mobile
slug: carnival-mobile-domain-security
source_filename: carnival-mobile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meetmarigold.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:37:08 2026 GMT\n  hsts: false\n- host: sdkdevelopers.meetmarigold.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 20:59:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: meetmarigold.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carnival-mobile/refs/heads/main/security/carnival-mobile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Mobile
- Push Notifications
- In-App Messaging
- Marketing Automation
- Customer Engagement
- Mobile SDK
- Acquired
---
