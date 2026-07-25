---
api_specs:
- filename: jetify-pkg-api-openapi.yml
  format: yaml
  label: Jetify Pkg API
  slug: jetify-pkg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetify/refs/heads/main/openapi/jetify-pkg-api-openapi.yml
- filename: jetify-resolve-api-openapi.yml
  format: yaml
  label: Jetify Resolve API
  slug: jetify-resolve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetify/refs/heads/main/openapi/jetify-resolve-api-openapi.yml
- filename: jetify-search-api-openapi.yml
  format: yaml
  label: Jetify Search API
  slug: jetify-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetify/refs/heads/main/openapi/jetify-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: jetify.com
  spf: true
hosts:
- cert_expires: Oct  2 17:50:24 2026 GMT
  host: www.jetify.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jetify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jetify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Jetify
provider_slug: jetify
slug: jetify-domain-security
source_filename: jetify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jetify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:50:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: jetify.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetify/refs/heads/main/security/jetify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Developer Tools
- Nix
- Package Management
- Developer Environments
- Reproducible Builds
- CLI
- Search
---
