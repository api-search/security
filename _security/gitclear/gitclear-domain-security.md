---
api_specs:
- filename: gitclear-api-tokens-api-openapi.yml
  format: yaml
  label: GitClear API Tokens API
  slug: gitclear-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-api-tokens-api-openapi.yml
- filename: gitclear-code-introspection-api-openapi.yml
  format: yaml
  label: GitClear Code Introspection API
  slug: gitclear-code-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-code-introspection-api-openapi.yml
- filename: gitclear-data-audit-api-openapi.yml
  format: yaml
  label: GitClear Data Audit API
  slug: gitclear-data-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-data-audit-api-openapi.yml
- filename: gitclear-developers-api-openapi.yml
  format: yaml
  label: GitClear Developers API
  slug: gitclear-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-developers-api-openapi.yml
- filename: gitclear-imports-api-openapi.yml
  format: yaml
  label: GitClear Imports API
  slug: gitclear-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-imports-api-openapi.yml
- filename: gitclear-releases-api-openapi.yml
  format: yaml
  label: GitClear Releases API
  slug: gitclear-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-releases-api-openapi.yml
- filename: gitclear-reports-api-openapi.yml
  format: yaml
  label: GitClear Reports API
  slug: gitclear-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-reports-api-openapi.yml
- filename: gitclear-teams-api-openapi.yml
  format: yaml
  label: GitClear Teams API
  slug: gitclear-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-teams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitclear.com
  spf: true
hosts:
- cert_expires: Sep 30 17:18:34 2026 GMT
  host: www.gitclear.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gitclear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitClear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GitClear
provider_slug: gitclear
slug: gitclear-domain-security
source_filename: gitclear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gitclear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 17:18:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gitclear.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/security/gitclear-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Code Analytics
- Commit Analytics
- Developer Productivity
- Diff Delta
- Engineering Metrics
---
