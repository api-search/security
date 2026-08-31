---
api_specs:
- filename: bump-sh-branches-api-openapi.yml
  format: yaml
  label: Bump.sh Branches API
  slug: bump-sh-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-branches-api-openapi.yml
- filename: bump-sh-diffs-api-openapi.yml
  format: yaml
  label: Bump.sh Diffs API
  slug: bump-sh-diffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-diffs-api-openapi.yml
- filename: bump-sh-hubs-api-openapi.yml
  format: yaml
  label: Bump.sh Hubs API
  slug: bump-sh-hubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-hubs-api-openapi.yml
- filename: bump-sh-mcp-servers-api-openapi.yml
  format: yaml
  label: Bump.sh MCP servers API
  slug: bump-sh-mcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-mcp-servers-api-openapi.yml
- filename: bump-sh-ping-api-openapi.yml
  format: yaml
  label: Bump.sh Ping API
  slug: bump-sh-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-ping-api-openapi.yml
- filename: bump-sh-previews-api-openapi.yml
  format: yaml
  label: Bump.sh Previews API
  slug: bump-sh-previews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-previews-api-openapi.yml
- filename: bump-sh-validations-api-openapi.yml
  format: yaml
  label: Bump.sh Validations API
  slug: bump-sh-validations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-validations-api-openapi.yml
- filename: bump-sh-versions-api-openapi.yml
  format: yaml
  label: Bump.sh Versions API
  slug: bump-sh-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-versions-api-openapi.yml
- filename: bump-sh-documentation-change-api-openapi.yml
  format: yaml
  label: Bump.sh Documentation change API
  slug: bump-sh-documentation-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-documentation-change-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bump.sh
  spf: true
hosts:
- cert_expires: Aug 21 14:54:42 2026 GMT
  host: bump.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bump Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bump.sh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bump.sh
provider_slug: bump-sh
slug: bump-sh-domain-security
source_filename: bump-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bump.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 14:54:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bump.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/security/bump-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Changelog
- API Documentation
- API Hub
- API Governance
- Arazzo
- AsyncAPI
- CI/CD
- Flower
- MCP
- OpenAPI
- Workflows
---
