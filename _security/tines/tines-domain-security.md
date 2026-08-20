---
api_specs:
- filename: tines-actions-api-openapi.yml
  format: yaml
  label: Tines Actions API
  slug: tines-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-actions-api-openapi.yml
- filename: tines-audit-logs-api-openapi.yml
  format: yaml
  label: Tines Audit Logs API
  slug: tines-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-audit-logs-api-openapi.yml
- filename: tines-credentials-api-openapi.yml
  format: yaml
  label: Tines Credentials API
  slug: tines-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-credentials-api-openapi.yml
- filename: tines-folders-api-openapi.yml
  format: yaml
  label: Tines Folders API
  slug: tines-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-folders-api-openapi.yml
- filename: tines-stories-api-openapi.yml
  format: yaml
  label: Tines Stories API
  slug: tines-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-stories-api-openapi.yml
- filename: tines-tags-api-openapi.yml
  format: yaml
  label: Tines Tags API
  slug: tines-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-tags-api-openapi.yml
- filename: tines-teams-api-openapi.yml
  format: yaml
  label: Tines Teams API
  slug: tines-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-teams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tines.com
  spf: true
hosts:
- cert_expires: Sep 15 03:58:04 2026 GMT
  host: www.tines.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tines
provider_slug: tines
slug: tines-domain-security
source_filename: tines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:58:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tines.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/security/tines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security Automation
- No-Code
- Workflow-Automation
- Security Operations
- SOAR
- Incident Response
- REST API
- Webhook
---
