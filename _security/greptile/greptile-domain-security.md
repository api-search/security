---
api_specs:
- filename: greptile-openapi.yml
  format: yaml
  label: Greptile Query API
  slug: greptile-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/openapi/greptile-openapi.yml
- filename: greptile-openapi.yml
  format: yaml
  label: Greptile Repositories (Indexing) API
  slug: greptile-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/openapi/greptile-openapi.yml
- filename: greptile-openapi.yml
  format: yaml
  label: Greptile Search API
  slug: greptile-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/openapi/greptile-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: greptile.com
  spf: true
hosts:
- cert_expires: Sep 14 11:06:56 2026 GMT
  host: www.greptile.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: docs.greptile.com
  https: false
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.greptile.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greptile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greptile, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Greptile
provider_slug: greptile
slug: greptile-domain-security
source_filename: greptile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greptile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 11:06:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.greptile.com\n  https: false\n- host: api.greptile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: greptile.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/security/greptile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Codebase Understanding
- Code Review
- Code Search
- Developer Tools
---
