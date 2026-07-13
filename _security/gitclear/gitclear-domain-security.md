---
api_specs:
- filename: gitclear-openapi.yml
  format: yaml
  label: GitClear Repositories API
  slug: gitclear-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-openapi.yml
- filename: gitclear-openapi.yml
  format: yaml
  label: GitClear Commits API
  slug: gitclear-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-openapi.yml
- filename: gitclear-openapi.yml
  format: yaml
  label: GitClear Metrics & Diff Delta API
  slug: gitclear-metrics-diff-delta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-openapi.yml
- filename: gitclear-openapi.yml
  format: yaml
  label: GitClear Developers API
  slug: gitclear-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-openapi.yml
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
