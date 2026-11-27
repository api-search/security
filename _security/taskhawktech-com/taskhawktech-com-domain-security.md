---
api_specs:
- filename: taskhawktech-com-opaque-event-interface-openapi.json
  format: json
  label: TaskHawk Opaque Event Interface
  slug: taskhawk-opaque-event-interface
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taskhawktech-com/openapi/taskhawktech-com-opaque-event-interface-openapi.json
- filename: taskhawktech-com-billing-api-openapi.yml
  format: yaml
  label: TaskHawk Systems Billing API
  slug: taskhawktech-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taskhawktech-com/openapi/taskhawktech-com-billing-api-openapi.yml
- filename: taskhawktech-com-events-api-openapi.yml
  format: yaml
  label: TaskHawk Systems Events API
  slug: taskhawktech-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taskhawktech-com/openapi/taskhawktech-com-events-api-openapi.yml
- filename: taskhawktech-com-governance-api-openapi.yml
  format: yaml
  label: TaskHawk Systems Governance API
  slug: taskhawktech-com-governance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taskhawktech-com/openapi/taskhawktech-com-governance-api-openapi.yml
- filename: taskhawktech-com-media-api-openapi.yml
  format: yaml
  label: TaskHawk Systems Media API
  slug: taskhawktech-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taskhawktech-com/openapi/taskhawktech-com-media-api-openapi.yml
- filename: taskhawktech-com-shield-api-openapi.yml
  format: yaml
  label: TaskHawk Systems Shield API
  slug: taskhawktech-com-shield-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taskhawktech-com/openapi/taskhawktech-com-shield-api-openapi.yml
- filename: taskhawktech-com-signup-api-openapi.yml
  format: yaml
  label: TaskHawk Systems Signup API
  slug: taskhawktech-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taskhawktech-com/openapi/taskhawktech-com-signup-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: taskhawktech.com
  spf: true
hosts:
- cert_expires: Jan 20 12:51:19 2027 GMT
  host: taskhawktech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: governance.taskhawktech.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: TaskHawk Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TaskHawk Systems, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TaskHawk Systems
provider_slug: taskhawktech-com
slug: taskhawktech-com-domain-security
source_filename: taskhawktech-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taskhawktech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 12:51:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: governance.taskhawktech.com\n  https: false\ndomains:\n- domain: taskhawktech.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/taskhawktech-com/security/taskhawktech-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Governance
- Agent Security
- Runtime Enforcement
- Policy Enforcement
- Provenance
- Compliance
- Prompt Injection Detection
- Media Attestation
- Post-Quantum Cryptography
- Formal Verification
- x402
- L402
- Machine Payments
- MCP
- A2A
- Agent-Native
- Government
- Defense
---
