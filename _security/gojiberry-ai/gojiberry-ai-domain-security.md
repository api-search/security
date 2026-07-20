---
api_specs:
- filename: gojiberry-ai-external-openapi-original.json
  format: json
  label: Gojiberry AI External API
  slug: gojiberry-ai-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-external-openapi-original.json
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
