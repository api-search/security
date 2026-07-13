---
api_specs:
- filename: suprsend-rest-api-openapi.yml
  format: yaml
  label: SuprSend REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suprsend/refs/heads/main/openapi/suprsend-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: suprsend.com
  spf: true
hosts:
- cert_expires: Sep 10 15:03:07 2026 GMT
  host: www.suprsend.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 01:43:38 2026 GMT
  host: docs.suprsend.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 18:17:07 2026 GMT
  host: hub.suprsend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Suprsend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SuprSend, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SuprSend
provider_slug: suprsend
slug: suprsend-domain-security
source_filename: suprsend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.suprsend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:03:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.suprsend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 01:43:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: hub.suprsend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 18:17:07 2026 GMT\n  hsts: null\ndomains:\n- domain: suprsend.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suprsend/refs/heads/main/security/suprsend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Notifications
- Multi-Channel
- Email
- SMS
- Push Notifications
- In-App Inbox
- WhatsApp
- Slack
- Notification Infrastructure
- Workflow Automation
- Template Management
---
