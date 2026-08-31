---
api_specs:
- filename: scalable-platforms-artifacts-api-openapi.yml
  format: yaml
  label: Scalable Platforms Artifacts API
  slug: scalable-platforms-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-artifacts-api-openapi.yml
- filename: scalable-platforms-deployments-api-openapi.yml
  format: yaml
  label: Scalable Platforms Deployments API
  slug: scalable-platforms-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-deployments-api-openapi.yml
- filename: scalable-platforms-domains-api-openapi.yml
  format: yaml
  label: Scalable Platforms Domains API
  slug: scalable-platforms-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-domains-api-openapi.yml
- filename: scalable-platforms-environments-api-openapi.yml
  format: yaml
  label: Scalable Platforms Environments API
  slug: scalable-platforms-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-environments-api-openapi.yml
- filename: scalable-platforms-projects-api-openapi.yml
  format: yaml
  label: Scalable Platforms Projects API
  slug: scalable-platforms-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-projects-api-openapi.yml
- filename: scalable-platforms-teams-api-openapi.yml
  format: yaml
  label: Scalable Platforms Teams API
  slug: scalable-platforms-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-teams-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vercel.com
  spf: true
hosts:
- cert_expires: Aug 21 08:55:49 2026 GMT
  host: api.vercel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scalable Platforms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scalable Platforms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scalable Platforms
provider_slug: scalable-platforms
slug: scalable-platforms-domain-security
source_filename: scalable-platforms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.vercel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 08:55:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vercel.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/security/scalable-platforms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Infrastructure
- Deployment
- Developer Experience
- DevOps
- PaaS
- Platform
- Scalability
- Serverless
---
