---
api_specs:
- filename: T17KeScV
  format: yaml
  label: Appgain OmniChannel Messaging API
  slug: appgain-omnichannel-messaging-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/4679101/T17KeScV?version=latest
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appgain.io
  spf: true
hosts:
- cert_expires: Sep  2 14:16:59 2026 GMT
  host: appgain.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 14:02:58 2026 GMT
  host: apidocs.appgain.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 11:08:16 2026 GMT
  host: api.appgain.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appgain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appgain, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Appgain
provider_slug: appgain
slug: appgain-domain-security
source_filename: appgain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appgain.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 14:16:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidocs.appgain.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 14:02:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.appgain.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 11:08:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: appgain.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appgain/refs/heads/main/security/appgain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobile Marketing
- Marketing Automation
- Omnichannel Messaging
- Push Notifications
- SMS
- Email
- WhatsApp
- Customer Data Platform
- Deep Linking
- Customer Engagement
---
