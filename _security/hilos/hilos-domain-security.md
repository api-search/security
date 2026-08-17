---
api_specs:
- filename: hilos-contact-api-openapi.yml
  format: yaml
  label: Hilos Contact API
  slug: hilos-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilos/refs/heads/main/openapi/hilos-contact-api-openapi.yml
- filename: hilos-conversation-api-openapi.yml
  format: yaml
  label: Hilos Conversation API
  slug: hilos-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilos/refs/heads/main/openapi/hilos-conversation-api-openapi.yml
- filename: hilos-flow-execution-api-openapi.yml
  format: yaml
  label: Hilos Flow Execution API
  slug: hilos-flow-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilos/refs/heads/main/openapi/hilos-flow-execution-api-openapi.yml
- filename: hilos-flow-execution-contact-api-openapi.yml
  format: yaml
  label: Hilos Flow Execution Contact API
  slug: hilos-flow-execution-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilos/refs/heads/main/openapi/hilos-flow-execution-contact-api-openapi.yml
- filename: hilos-user-api-openapi.yml
  format: yaml
  label: Hilos User API
  slug: hilos-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilos/refs/heads/main/openapi/hilos-user-api-openapi.yml
- filename: hilos-whatsapp-api-openapi.yml
  format: yaml
  label: Hilos WhatsApp API
  slug: hilos-whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilos/refs/heads/main/openapi/hilos-whatsapp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hilos.io
  spf: false
hosts:
- cert_expires: Oct  8 06:08:48 2026 GMT
  host: hilos.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 06:08:48 2026 GMT
  host: api.hilos.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hilos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hilos, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Hilos
provider_slug: hilos
slug: hilos-domain-security
source_filename: hilos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hilos.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 06:08:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hilos.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 06:08:48 2026 GMT\n  hsts: null\ndomains:\n- domain: hilos.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hilos/refs/heads/main/security/hilos-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- WhatsApp
- Messaging
- Automation
- CRM
- Conversational Commerce
- Chatbots
- Customer Engagement
- Marketing
---
