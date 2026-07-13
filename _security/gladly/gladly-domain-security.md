---
api_specs:
- filename: gladly-rest-api-openapi.yml
  format: yaml
  label: Gladly REST API
  slug: gladly-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/openapi/gladly-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gladly.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gladly.com
  spf: true
hosts:
- cert_expires: Aug 17 00:58:11 2026 GMT
  host: www.gladly.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 13:11:19 2026 GMT
  host: developer.gladly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: organization.gladly.com
  https: false
kind: domain-security
layout: security
method: probed
name: Gladly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gladly, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gladly
provider_slug: gladly
slug: gladly-domain-security
source_filename: gladly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gladly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 00:58:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.gladly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:11:19 2026 GMT\n  hsts: false\n- host: organization.gladly.com\n  https: false\ndomains:\n- domain: gladly.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gladly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/security/gladly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Service
- CX
- Contact Center
- AI Customer Service
- Conversations
- Sidekick AI
- Hero
- Voice
- Chat
- SMS
- Email
- Help Center
- Webhooks
- Knowledge Base
---
