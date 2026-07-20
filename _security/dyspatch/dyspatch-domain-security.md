---
api_specs:
- filename: dyspatch-openapi-original.json
  format: json
  label: Dyspatch API
  slug: dyspatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyspatch/refs/heads/main/openapi/dyspatch-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dyspatch.io
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: api.dyspatch.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dyspatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dyspatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dyspatch
provider_slug: dyspatch
slug: dyspatch-domain-security
source_filename: dyspatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.dyspatch.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dyspatch.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dyspatch/refs/heads/main/security/dyspatch-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Email
- Email Templates
- Marketing
- Messaging
- SMS
- Push Notifications
- Localization
- Content Management
- Developer Tools
---
