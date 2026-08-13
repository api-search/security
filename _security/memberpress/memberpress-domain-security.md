---
api_specs:
- filename: memberpress-developer-tools-openapi.yml
  format: yaml
  label: MemberPress Developer Tools REST API
  slug: developer-tools-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/openapi/memberpress-developer-tools-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: memberpress.com
  spf: true
hosts:
- cert_expires: Oct  3 16:59:27 2026 GMT
  host: memberpress.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memberpress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MemberPress, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MemberPress
provider_slug: memberpress
slug: memberpress-domain-security
source_filename: memberpress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memberpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:59:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: memberpress.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/security/memberpress-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Membership
- Subscriptions
- WordPress
- Payments
- E-Commerce
- Courses
- Content Management
- Webhooks
- MCP
---
