---
api_specs:
- filename: release-accounts-api-openapi.yml
  format: yaml
  label: Release Accounts API
  slug: release-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/release/refs/heads/main/openapi/release-accounts-api-openapi.yml
- filename: release-apps-api-openapi.yml
  format: yaml
  label: Release Apps API
  slug: release-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/release/refs/heads/main/openapi/release-apps-api-openapi.yml
- filename: release-builds-api-openapi.yml
  format: yaml
  label: Release Builds API
  slug: release-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/release/refs/heads/main/openapi/release-builds-api-openapi.yml
- filename: release-clusters-api-openapi.yml
  format: yaml
  label: Release Clusters API
  slug: release-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/release/refs/heads/main/openapi/release-clusters-api-openapi.yml
- filename: release-configs-api-openapi.yml
  format: yaml
  label: Release Configs API
  slug: release-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/release/refs/heads/main/openapi/release-configs-api-openapi.yml
- filename: release-deploys-api-openapi.yml
  format: yaml
  label: Release Deploys API
  slug: release-deploys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/release/refs/heads/main/openapi/release-deploys-api-openapi.yml
- filename: release-environments-api-openapi.yml
  format: yaml
  label: Release Environments API
  slug: release-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/release/refs/heads/main/openapi/release-environments-api-openapi.yml
- filename: release-instances-api-openapi.yml
  format: yaml
  label: Release Instances API
  slug: release-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/release/refs/heads/main/openapi/release-instances-api-openapi.yml
- filename: release-remote-development-api-openapi.yml
  format: yaml
  label: Release Remote Development API
  slug: release-remote-development-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/release/refs/heads/main/openapi/release-remote-development-api-openapi.yml
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
