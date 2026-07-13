---
api_specs:
- filename: paragon-proxy-api-openapi.yml
  format: yaml
  label: Proxy API
  slug: proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-proxy-api-openapi.yml
- filename: paragon-users-api-openapi.yml
  format: yaml
  label: Users API
  slug: users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-users-api-openapi.yml
- filename: paragon-task-history-api-openapi.yml
  format: yaml
  label: Task History API
  slug: task-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-task-history-api-openapi.yml
- filename: paragon-actionkit-api-openapi.yml
  format: yaml
  label: ActionKit API
  slug: actionkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-actionkit-api-openapi.yml
- filename: paragon-triggers-api-openapi.yml
  format: yaml
  label: Triggers API
  slug: triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-triggers-api-openapi.yml
- filename: paragon-managed-sync-api-openapi.yml
  format: yaml
  label: Managed Sync API
  slug: managed-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/openapi/paragon-managed-sync-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: useparagon.com
  spf: true
hosts:
- cert_expires: Sep  7 00:16:04 2026 GMT
  host: docs.useparagon.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 05:33:24 2026 GMT
  host: actionkit.useparagon.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: managed-sync.useparagon.com
  https: false
kind: domain-security
layout: security
method: probed
name: Paragon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paragon, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paragon
provider_slug: paragon
slug: paragon-domain-security
source_filename: paragon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.useparagon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 00:16:04 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: actionkit.useparagon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:33:24 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: managed-sync.useparagon.com\n  https: false\ndomains:\n- domain: useparagon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/security/paragon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Embedded Integrations
- Integration Infrastructure
- iPaaS
- AI Agents
- MCP
- Integrations
---
