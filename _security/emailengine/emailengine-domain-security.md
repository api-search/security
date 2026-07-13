---
api_specs:
- filename: emailengine-openapi.yml
  format: yaml
  label: EmailEngine API
  slug: emailengine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: emailengine.app
  spf: true
hosts:
- cert_expires: Aug 30 23:10:39 2026 GMT
  host: emailengine.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 16:22:24 2026 GMT
  host: api.emailengine.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emailengine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EmailEngine, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EmailEngine
provider_slug: emailengine
slug: emailengine-domain-security
source_filename: emailengine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emailengine.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:10:39 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.emailengine.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 16:22:24 2026 GMT\n  hsts: false\ndomains:\n- domain: emailengine.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/security/emailengine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Email API
- IMAP
- SMTP
- Webhooks
---
