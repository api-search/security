---
api_specs:
- filename: introduction
  format: yaml
  label: Engagespot Notifications API
  slug: notifications-api
  spec_type: OpenAPI
  url: https://docs.engagespot.co/api/api-reference/introduction
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: engagespot.co
  spf: true
hosts:
- cert_expires: Sep 19 13:50:17 2026 GMT
  host: engagespot.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 18:33:45 2026 GMT
  host: docs.engagespot.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.engagespot.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Engagespot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Engagespot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Engagespot
provider_slug: engagespot
slug: engagespot-domain-security
source_filename: engagespot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: engagespot.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 13:50:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.engagespot.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 18:33:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.engagespot.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: engagespot.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engagespot/refs/heads/main/security/engagespot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notifications
- In-App Notifications
- Push Notifications
- Email
- SMS
- Multi-Channel
- Messaging
- Developer Tools
- Notification Infrastructure
---
