---
api_specs:
- filename: conversica-integrations-api-openapi.yml
  format: yaml
  label: Conversica Integrations API
  slug: integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conversica/refs/heads/main/openapi/conversica-integrations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: conversica.com
  spf: true
hosts:
- cert_expires: Oct  4 20:29:02 2026 GMT
  host: www.conversica.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:41:41 2026 GMT
  host: help.conversica.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: integrations-api.conversica.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conversica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conversica, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Conversica
provider_slug: conversica
slug: conversica-domain-security
source_filename: conversica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conversica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 20:29:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.conversica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:41:41 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: integrations-api.conversica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: conversica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conversica/refs/heads/main/security/conversica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Conversational AI
- AI Agents
- Sales
- Marketing
- Lead Management
- CRM
- Marketing Automation
- Customer Engagement
- Messaging
- SMS
- Email
- Chat
- Automotive
- Higher Education
- Webhook
---
