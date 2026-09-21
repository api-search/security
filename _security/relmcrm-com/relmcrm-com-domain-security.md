---
api_specs:
- filename: relmcrm-com-openapi.yml
  format: yaml
  label: Relm CRM REST API
  slug: relm-crm-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: relmcrm.com
  spf: true
hosts:
- cert_expires: Nov 28 20:04:17 2026 GMT
  host: relmcrm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 20:04:17 2026 GMT
  host: api.relmcrm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Relmcrm Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relm, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Relm
provider_slug: relmcrm-com
slug: relmcrm-com-domain-security
source_filename: relmcrm-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: relmcrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 20:04:17 2026 GMT\n  hsts: false\n- host: api.relmcrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 20:04:17 2026 GMT\n  hsts: false\ndomains:\n- domain: relmcrm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/security/relmcrm-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CRM
- Sales
- Contacts
- Deals
- Sales Pipeline
- Automation
- Webhook
- MCP
- A2A
- AI Agents
- agent-native
- United Arab Emirates
---
