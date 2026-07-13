---
api_specs:
- filename: bump-sh-openapi.yaml
  format: yaml
  label: Bump.sh API
  slug: bump-sh-api
  spec_type: OpenAPI
  url: https://github.com/api-evangelist/bump-sh/blob/main/openapi/bump-sh-openapi.yaml
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
