---
api_specs:
- filename: teamcity-rest-api.yml
  format: yaml
  label: TeamCity REST API
  slug: teamcity-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-rest-api.yml
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
kind: domain-security
layout: security
method: probed
name: Teamcity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TeamCity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TeamCity
provider_slug: teamcity
slug: teamcity-domain-security
source_filename: teamcity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jetbrains.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jetbrains.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/security/teamcity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Build Automation
- CI/CD
- Continuous Integration
- Deployment
- DevOps
- Testing
---
