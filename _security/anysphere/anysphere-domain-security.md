---
api_specs:
- filename: anysphere-agents-api-openapi.yml
  format: yaml
  label: Anysphere Agents API
  slug: anysphere-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anysphere/refs/heads/main/openapi/anysphere-agents-api-openapi.yml
- filename: anysphere-me-api-openapi.yml
  format: yaml
  label: Anysphere Me API
  slug: anysphere-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anysphere/refs/heads/main/openapi/anysphere-me-api-openapi.yml
- filename: anysphere-models-api-openapi.yml
  format: yaml
  label: Anysphere Models API
  slug: anysphere-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anysphere/refs/heads/main/openapi/anysphere-models-api-openapi.yml
- filename: anysphere-repositories-api-openapi.yml
  format: yaml
  label: Anysphere Repositories API
  slug: anysphere-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anysphere/refs/heads/main/openapi/anysphere-repositories-api-openapi.yml
- filename: anysphere-sub-tokens-api-openapi.yml
  format: yaml
  label: Anysphere Sub Tokens API
  slug: anysphere-sub-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anysphere/refs/heads/main/openapi/anysphere-sub-tokens-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anysphere.inc
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cursor.com
  spf: true
hosts:
- cert_expires: Sep 20 02:36:25 2026 GMT
  host: anysphere.inc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: api.cursor.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Anysphere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anysphere, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Anysphere
provider_slug: anysphere
slug: anysphere-domain-security
source_filename: anysphere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anysphere.inc\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 02:36:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cursor.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: anysphere.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cursor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anysphere/refs/heads/main/security/anysphere-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Artificial Intelligence
- Code Editor
- Coding Agents
- Cloud Agents
- Developer Productivity
- IDE
---
