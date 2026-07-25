---
api_specs:
- filename: nevercode-app-previews-api-openapi.yml
  format: yaml
  label: Nevercode App Previews API
  slug: nevercode-app-previews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-app-previews-api-openapi.yml
- filename: nevercode-applications-api-openapi.yml
  format: yaml
  label: Nevercode Applications API
  slug: nevercode-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-applications-api-openapi.yml
- filename: nevercode-billing-api-openapi.yml
  format: yaml
  label: Nevercode Billing API
  slug: nevercode-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-billing-api-openapi.yml
- filename: nevercode-build-dashboards-api-openapi.yml
  format: yaml
  label: Nevercode Build Dashboards API
  slug: nevercode-build-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-build-dashboards-api-openapi.yml
- filename: nevercode-builds-api-openapi.yml
  format: yaml
  label: Nevercode Builds API
  slug: nevercode-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-builds-api-openapi.yml
- filename: nevercode-meta-api-openapi.yml
  format: yaml
  label: Nevercode Meta API
  slug: nevercode-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-meta-api-openapi.yml
- filename: nevercode-over-the-air-updates-api-openapi.yml
  format: yaml
  label: Nevercode Over-the-air Updates API
  slug: nevercode-over-the-air-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-over-the-air-updates-api-openapi.yml
- filename: nevercode-secrets-and-environment-vars-api-openapi.yml
  format: yaml
  label: Nevercode Secrets and Environment Vars API
  slug: nevercode-secrets-and-environment-vars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-secrets-and-environment-vars-api-openapi.yml
- filename: nevercode-team-invitations-api-openapi.yml
  format: yaml
  label: Nevercode Team Invitations API
  slug: nevercode-team-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-team-invitations-api-openapi.yml
- filename: nevercode-team-members-api-openapi.yml
  format: yaml
  label: Nevercode Team Members API
  slug: nevercode-team-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-team-members-api-openapi.yml
- filename: nevercode-teams-api-openapi.yml
  format: yaml
  label: Nevercode Teams API
  slug: nevercode-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-teams-api-openapi.yml
- filename: nevercode-tester-groups-api-openapi.yml
  format: yaml
  label: Nevercode Tester Groups API
  slug: nevercode-tester-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-tester-groups-api-openapi.yml
- filename: nevercode-users-api-openapi.yml
  format: yaml
  label: Nevercode Users API
  slug: nevercode-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: codemagic.io
  spf: true
hosts:
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: codemagic.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: docs.codemagic.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nevercode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nevercode, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nevercode
provider_slug: nevercode
slug: nevercode-domain-security
source_filename: nevercode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codemagic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.codemagic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: codemagic.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/security/nevercode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Continuous Integration
- Continuous Delivery
- CI/CD
- DevOps
- Mobile
- Flutter
- Builds
- App Distribution
- Code Signing
---
