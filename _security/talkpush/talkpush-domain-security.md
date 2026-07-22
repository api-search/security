---
api_specs:
- filename: talkpush-openapi.json
  format: json
  label: Talkpush API
  slug: talkpush-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: talkpush.com
  spf: true
hosts:
- cert_expires: Sep 28 16:53:32 2026 GMT
  host: www.talkpush.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: docs.talkpush.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: your-company.talkpush.com
  https: false
kind: domain-security
layout: security
method: probed
name: Talkpush Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TalkPush, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: TalkPush
provider_slug: talkpush
slug: talkpush-domain-security
source_filename: talkpush-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.talkpush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:53:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.talkpush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-company.talkpush.com\n  https: false\ndomains:\n- domain: talkpush.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/security/talkpush-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Recruiting
- Recruitment Automation
- Human Resources
- Hiring
- Applicant Tracking
- Conversational AI
- Messaging
- CRM
---
