---
api_specs:
- filename: chatway-app-openapi-generated.yml
  format: yaml
  label: Chatway API
  slug: chatway-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatway-app/openapi/_ae-authored/chatway-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chatway.app
  spf: true
hosts:
- cert_expires: Dec 17 09:31:51 2026 GMT
  host: chatway.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chatway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chatway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chatway
provider_slug: chatway-app
slug: chatway-app-domain-security
source_filename: chatway-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chatway.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 09:31:51 2026 GMT\n  hsts: false\ndomains:\n- domain: chatway.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chatway-app/security/chatway-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Live Chat
- Artificial Intelligence
- Customer Service
- MCP
- Chatbots
- Company
---
