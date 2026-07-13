---
api_specs:
- filename: crisp-openapi.yml
  format: yaml
  label: Crisp REST API v1
  slug: crisp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crisp/refs/heads/main/openapi/crisp-openapi.yml
- filename: crisp-asyncapi.yml
  format: yaml
  label: Crisp Realtime (Webhooks + RTM) v1
  slug: crisp-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/crisp/refs/heads/main/asyncapi/crisp-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: crisp.chat
  spf: true
hosts:
- cert_expires: Aug 16 11:43:54 2026 GMT
  host: crisp.chat
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 11:43:54 2026 GMT
  host: docs.crisp.chat
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 11:43:54 2026 GMT
  host: api.crisp.chat
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crisp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crisp, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Crisp
provider_slug: crisp
slug: crisp-domain-security
source_filename: crisp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crisp.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 11:43:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.crisp.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 11:43:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.crisp.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 11:43:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crisp.chat\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crisp/refs/heads/main/security/crisp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Customer Service
- Live Chat
- Helpdesk
- Messaging
- Chatbots
---
