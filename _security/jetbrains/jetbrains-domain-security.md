---
api_specs:
- filename: jetbrains-space-openapi.yml
  format: yaml
  label: JetBrains Space HTTP API
  slug: space-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/openapi/jetbrains-space-openapi.yml
- filename: jetbrains-teamcity-openapi.yml
  format: yaml
  label: JetBrains TeamCity REST API
  slug: teamcity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/openapi/jetbrains-teamcity-openapi.yml
- filename: jetbrains-youtrack-openapi.yml
  format: yaml
  label: JetBrains YouTrack REST API
  slug: youtrack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/openapi/jetbrains-youtrack-openapi.yml
- filename: jetbrains-hub-openapi.yml
  format: yaml
  label: JetBrains Hub REST API
  slug: hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/openapi/jetbrains-hub-openapi.yml
- filename: jetbrains-marketplace-openapi.yml
  format: yaml
  label: JetBrains Marketplace API
  slug: marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/openapi/jetbrains-marketplace-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jetbrains.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.jetbrains.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: plugins.jetbrains.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jetbrains Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JetBrains, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JetBrains
provider_slug: jetbrains
slug: jetbrains-domain-security
source_filename: jetbrains-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jetbrains.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: plugins.jetbrains.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jetbrains.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/security/jetbrains-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CI/CD
- Developer Tools
- IDE
---
