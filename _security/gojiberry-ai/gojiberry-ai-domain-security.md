---
api_specs:
- filename: gojiberry-ai-appexternal-api-openapi.yml
  format: yaml
  label: Gojiberry AI AppExternal API
  slug: gojiberry-ai-appexternal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-appexternal-api-openapi.yml
- filename: gojiberry-ai-campaigns-api-openapi.yml
  format: yaml
  label: Gojiberry AI Campaigns API
  slug: gojiberry-ai-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-campaigns-api-openapi.yml
- filename: gojiberry-ai-contacts-api-openapi.yml
  format: yaml
  label: Gojiberry AI Contacts API
  slug: gojiberry-ai-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-contacts-api-openapi.yml
- filename: gojiberry-ai-lead-source-agents-api-openapi.yml
  format: yaml
  label: Gojiberry AI Lead source agents API
  slug: gojiberry-ai-lead-source-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-lead-source-agents-api-openapi.yml
- filename: gojiberry-ai-lists-api-openapi.yml
  format: yaml
  label: Gojiberry AI Lists API
  slug: gojiberry-ai-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-lists-api-openapi.yml
- filename: gojiberry-ai-organization-api-openapi.yml
  format: yaml
  label: Gojiberry AI Organization API
  slug: gojiberry-ai-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-organization-api-openapi.yml
- filename: gojiberry-ai-unibox-api-openapi.yml
  format: yaml
  label: Gojiberry AI Unibox API
  slug: gojiberry-ai-unibox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-unibox-api-openapi.yml
- filename: gojiberry-ai-user-api-openapi.yml
  format: yaml
  label: Gojiberry AI User API
  slug: gojiberry-ai-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-user-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gojiberry.ai
  spf: true
hosts:
- cert_expires: Sep 27 14:32:39 2026 GMT
  host: gojiberry.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 14:32:39 2026 GMT
  host: app.gojiberry.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: ext.gojiberry.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gojiberry Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gojiberry AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gojiberry AI
provider_slug: gojiberry-ai
slug: gojiberry-ai-domain-security
source_filename: gojiberry-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gojiberry.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:32:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.gojiberry.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:32:39 2026 GMT\n  hsts: false\n- host: ext.gojiberry.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gojiberry.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/security/gojiberry-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sales
- Lead Generation
- Sales Intelligence
- AI Agents
- Outbound
- Go-To-Market
- Prospecting
- LinkedIn
- CRM
---
