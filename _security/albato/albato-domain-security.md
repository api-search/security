---
api_specs:
- filename: albato-automations-openapi.yaml
  format: yaml
  label: Albato Automations API
  slug: automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/openapi/albato-automations-openapi.yaml
- filename: albato-embedded-openapi.yaml
  format: yaml
  label: Albato Embedded API
  slug: embedded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/openapi/albato-embedded-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: albato.com
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: albato.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Albato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Albato, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Albato
provider_slug: albato
slug: albato-domain-security
source_filename: albato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: albato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: albato.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/security/albato-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- No-Code Automation
- Workflow Automation
- Embedded iPaaS
- App Integration
- Integrations
- Webhooks
- White-Label
---
