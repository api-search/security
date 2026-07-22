---
api_specs:
- filename: release-openapi-original.json
  format: json
  label: Release Platform API
  slug: release-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/release/refs/heads/main/openapi/release-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: release.com
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: release.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: api.release.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Release Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Release, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Release
provider_slug: release
slug: release-domain-security
source_filename: release-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: release.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.release.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: release.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/release/refs/heads/main/security/release-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Ephemeral Environments
- Platform Engineering
- Deployment
- Kubernetes
- Environments as a Service
- DevOps
- CI/CD
- AI Sandbox
---
