---
api_specs:
- filename: getvocal-contact-api-openapi.yml
  format: yaml
  label: GetVocal Contact API
  slug: getvocal-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvocal/refs/heads/main/openapi/getvocal-contact-api-openapi.yml
- filename: getvocal-llms-txt-api-openapi.yml
  format: yaml
  label: GetVocal Llms.txt API
  slug: getvocal-llms-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvocal/refs/heads/main/openapi/getvocal-llms-txt-api-openapi.yml
- filename: getvocal-well-known-api-openapi.yml
  format: yaml
  label: GetVocal .well Known API
  slug: getvocal-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvocal/refs/heads/main/openapi/getvocal-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getvocal.ai
  spf: true
hosts:
- cert_expires: Oct 13 22:31:12 2026 GMT
  host: www.getvocal.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getvocal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetVocal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GetVocal
provider_slug: getvocal
slug: getvocal-domain-security
source_filename: getvocal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getvocal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 22:31:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getvocal.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getvocal/refs/heads/main/security/getvocal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Voice AI
- Conversational AI
- Customer Experience
- AI Agents
- Contact Center
- Agent Governance
- MCP
- Agent Native
---
