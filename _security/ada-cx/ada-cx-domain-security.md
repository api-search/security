---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Ada REST API
  slug: ada-rest-api
  spec_type: OpenAPI
  url: https://docs.ada.cx/openapi.yaml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@ada.cx"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "amazonzonaws.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ada.cx
  spf: true
hosts:
- cert_expires: Aug 21 19:01:27 2026 GMT
  host: www.ada.cx
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 16:41:43 2026 GMT
  host: docs.ada.cx
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ada Cx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ada, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ada
provider_slug: ada-cx
slug: ada-cx-domain-security
source_filename: ada-cx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ada.cx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 19:01:27 2026 GMT\n  hsts: null\n- host: docs.ada.cx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 16:41:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ada.cx\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@ada.cx\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"amazonzonaws.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ada-cx/refs/heads/main/security/ada-cx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Agent
- Automation
- Chatbots
- Conversational AI
- Customer Service
- Customer Support
- CX
- Generative AI
- Knowledge
- Messaging
---
