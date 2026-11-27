---
api_specs:
- filename: modulos-ai-booking-api-openapi.yml
  format: yaml
  label: Modulos Booking API
  slug: modulos-ai-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modulos-ai/openapi/modulos-ai-booking-api-openapi.yml
- filename: modulos-ai-evaluation-api-openapi.yml
  format: yaml
  label: Modulos Evaluation API
  slug: modulos-ai-evaluation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modulos-ai/openapi/modulos-ai-evaluation-api-openapi.yml
- filename: modulos-ai-leads-api-openapi.yml
  format: yaml
  label: Modulos Leads API
  slug: modulos-ai-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modulos-ai/openapi/modulos-ai-leads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modulos.ai
  spf: true
hosts:
- cert_expires: Dec 19 19:19:42 2026 GMT
  host: modulos.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Modulos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modulos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Modulos
provider_slug: modulos-ai
slug: modulos-ai-domain-security
source_filename: modulos-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modulos.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 19:19:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: modulos.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/modulos-ai/security/modulos-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Governance
- Enterprise
- ISO 42001
- Risk Management
---
