---
api_specs:
- filename: postalform-com-machine-payments-openapi.json
  format: json
  label: PostalForm Machine Payments API
  slug: postalform-machine-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postalform-com/refs/heads/main/openapi/postalform-com-machine-payments-openapi.json
- filename: postalform-com-projects-openapi.json
  format: json
  label: PostalForm Projects Public API
  slug: postalform-projects-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postalform-com/refs/heads/main/openapi/postalform-com-projects-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: postalform.com
  spf: true
hosts:
- cert_expires: Nov 28 06:21:47 2026 GMT
  host: postalform.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 06:21:47 2026 GMT
  host: projects.postalform.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Postalform Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PostalForm, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PostalForm
provider_slug: postalform-com
slug: postalform-com-domain-security
source_filename: postalform-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: postalform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 06:21:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: projects.postalform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 06:21:47 2026 GMT\n  hsts: false\ndomains:\n- domain: postalform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postalform-com/refs/heads/main/security/postalform-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Physical Mail
- Print & Mail
- Postal Mail
- Certified Mail
- Documents
- Agents
- Agentic Commerce
- MCP
- A2A
- x402
- Machine Payments
- Webhook
- agent-native
- United States
---
