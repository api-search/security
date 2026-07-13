---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Loops API
  slug: loops-api
  spec_type: OpenAPI
  url: https://app.loops.so/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: loops.so
  spf: true
hosts:
- cert_expires: Sep 14 20:39:28 2026 GMT
  host: loops.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 18:48:26 2026 GMT
  host: app.loops.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loops So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loops, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Loops
provider_slug: loops-so
slug: loops-so-domain-security
source_filename: loops-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loops.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:39:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.loops.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:48:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: loops.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/security/loops-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Marketing Email
- Transactional Email
- Email Automation
- Email Campaigns
- Email Workflows
- Contacts
- Audience Management
- Events
- Webhooks
- SaaS
- Developer Tools
---
