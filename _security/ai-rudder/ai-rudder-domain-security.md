---
api_specs:
- filename: ai-rudder-openapi-generated.yml
  format: yaml
  label: AI Rudder API
  slug: ai-rudder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-rudder/openapi/_ae-authored/ai-rudder-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: airudder.com
  spf: true
hosts:
- cert_expires: Jan 13 20:47:02 2027 GMT
  host: airudder.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ai Rudder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Rudder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AI Rudder
provider_slug: ai-rudder
slug: ai-rudder-domain-security
source_filename: ai-rudder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airudder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 20:47:02 2027 GMT\n  hsts: false\ndomains:\n- domain: airudder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ai-rudder/security/ai-rudder-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- ConversationalAI
- Enterprise
- Automation
- Platform
---
