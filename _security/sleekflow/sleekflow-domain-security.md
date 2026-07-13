---
api_specs:
- filename: sleekflow-openapi.yml
  format: yaml
  label: SleekFlow Contacts API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/openapi/sleekflow-openapi.yml
- filename: sleekflow-openapi.yml
  format: yaml
  label: SleekFlow Conversations & Messaging API
  slug: conversations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/openapi/sleekflow-openapi.yml
- filename: sleekflow-openapi.yml
  format: yaml
  label: SleekFlow Companies API
  slug: companies
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/openapi/sleekflow-openapi.yml
- filename: sleekflow-openapi.yml
  format: yaml
  label: SleekFlow Lists API
  slug: lists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/openapi/sleekflow-openapi.yml
- filename: sleekflow-openapi.yml
  format: yaml
  label: SleekFlow Staff & Teams API
  slug: staff-teams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/openapi/sleekflow-openapi.yml
- filename: sleekflow-openapi.yml
  format: yaml
  label: SleekFlow Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/openapi/sleekflow-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sleekflow.io
  spf: true
hosts:
- cert_expires: Sep 22 08:58:38 2026 GMT
  host: sleekflow.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 22:10:18 2026 GMT
  host: apidoc.sleekflow.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 09:39:47 2026 GMT
  host: api.sleekflow.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sleekflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SleekFlow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SleekFlow
provider_slug: sleekflow
slug: sleekflow-domain-security
source_filename: sleekflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sleekflow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 08:58:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidoc.sleekflow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:10:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sleekflow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 09:39:47 2026 GMT\n  hsts: null\ndomains:\n- domain: sleekflow.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/security/sleekflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- Omnichannel
- WhatsApp
- Customer Engagement
- Social Commerce
- Automation
---
