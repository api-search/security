---
api_specs:
- filename: truto-admin-openapi.yml
  format: yaml
  label: Truto Admin API
  slug: truto-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-admin-openapi.yml
- filename: truto-unified-hris-openapi.yml
  format: yaml
  label: Truto Unified HRIS API
  slug: truto-unified-hris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-unified-hris-openapi.yml
- filename: truto-unified-ats-openapi.yml
  format: yaml
  label: Truto Unified ATS API
  slug: truto-unified-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-unified-ats-openapi.yml
- filename: truto-unified-crm-openapi.yml
  format: yaml
  label: Truto Unified CRM API
  slug: truto-unified-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-unified-crm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: truto.one
  spf: true
hosts:
- cert_expires: Oct  5 22:00:49 2026 GMT
  host: truto.one
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 12:16:56 2026 GMT
  host: api.truto.one
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truto, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Truto
provider_slug: truto
slug: truto-domain-security
source_filename: truto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truto.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:00:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.truto.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 12:16:56 2026 GMT\n  hsts: null\ndomains:\n- domain: truto.one\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/security/truto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Unified API
- Integration Platform
- HRIS
- ATS
- CRM
- Embedded Integrations
- MCP
- AI Agents
- SaaS
---
