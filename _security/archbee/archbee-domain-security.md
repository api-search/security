---
api_specs:
- filename: archbee-access-control-api-openapi.yml
  format: yaml
  label: Archbee Access Control API
  slug: archbee-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-access-control-api-openapi.yml
- filename: archbee-api-reference-api-openapi.yml
  format: yaml
  label: Archbee API Reference API
  slug: archbee-api-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-api-reference-api-openapi.yml
- filename: archbee-documents-api-openapi.yml
  format: yaml
  label: Archbee Documents API
  slug: archbee-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-documents-api-openapi.yml
- filename: archbee-file-manager-api-openapi.yml
  format: yaml
  label: Archbee File Manager API
  slug: archbee-file-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-file-manager-api-openapi.yml
- filename: archbee-members-api-openapi.yml
  format: yaml
  label: Archbee Members API
  slug: archbee-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-members-api-openapi.yml
- filename: archbee-organization-api-openapi.yml
  format: yaml
  label: Archbee Organization API
  slug: archbee-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-organization-api-openapi.yml
- filename: archbee-pages-api-openapi.yml
  format: yaml
  label: Archbee Pages API
  slug: archbee-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-pages-api-openapi.yml
- filename: archbee-space-groups-api-openapi.yml
  format: yaml
  label: Archbee Space Groups API
  slug: archbee-space-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-space-groups-api-openapi.yml
- filename: archbee-spaces-api-openapi.yml
  format: yaml
  label: Archbee Spaces API
  slug: archbee-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-spaces-api-openapi.yml
- filename: archbee-suggestions-api-openapi.yml
  format: yaml
  label: Archbee Suggestions API
  slug: archbee-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-suggestions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: archbee.com
  spf: true
hosts:
- cert_expires: Oct 11 05:50:00 2026 GMT
  host: www.archbee.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 22:00:25 2026 GMT
  host: api.archbee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Archbee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archbee, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Archbee
provider_slug: archbee
slug: archbee-domain-security
source_filename: archbee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.archbee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 05:50:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.archbee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 22:00:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: archbee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/security/archbee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
- Developer Portal
- Docs as Code
- OpenAPI
- MCP
- AI Agents
- Content Management
- Developer Tools
---
