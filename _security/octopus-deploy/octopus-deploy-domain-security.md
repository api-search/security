---
api_specs:
- filename: octopus-deploy-accounts-api-openapi.yml
  format: yaml
  label: Octopus Deploy Accounts API
  slug: octopus-deploy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octopus-deploy/refs/heads/main/openapi/octopus-deploy-accounts-api-openapi.yml
- filename: octopus-deploy-environments-api-openapi.yml
  format: yaml
  label: Octopus Deploy Environments API
  slug: octopus-deploy-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octopus-deploy/refs/heads/main/openapi/octopus-deploy-environments-api-openapi.yml
- filename: octopus-deploy-feeds-api-openapi.yml
  format: yaml
  label: Octopus Deploy Feeds API
  slug: octopus-deploy-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octopus-deploy/refs/heads/main/openapi/octopus-deploy-feeds-api-openapi.yml
- filename: octopus-deploy-machines-api-openapi.yml
  format: yaml
  label: Octopus Deploy Machines API
  slug: octopus-deploy-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octopus-deploy/refs/heads/main/openapi/octopus-deploy-machines-api-openapi.yml
- filename: octopus-deploy-projects-api-openapi.yml
  format: yaml
  label: Octopus Deploy Projects API
  slug: octopus-deploy-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octopus-deploy/refs/heads/main/openapi/octopus-deploy-projects-api-openapi.yml
- filename: octopus-deploy-root-api-openapi.yml
  format: yaml
  label: Octopus Deploy Root API
  slug: octopus-deploy-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octopus-deploy/refs/heads/main/openapi/octopus-deploy-root-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: octopus.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-octopus.example
  spf: false
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: octopus.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: your-octopus.example
  https: false
kind: domain-security
layout: security
method: probed
name: Octopus Deploy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octopus Deploy, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Octopus Deploy
provider_slug: octopus-deploy
slug: octopus-deploy-domain-security
source_filename: octopus-deploy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: octopus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: your-octopus.example\n  https: false\ndomains:\n- domain: octopus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: your-octopus.example\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octopus-deploy/refs/heads/main/security/octopus-deploy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DevOps
- Continuous Delivery
- Deployment Automation
- Release Management
- Runbooks
- CI/CD
---
