---
api_specs:
- filename: heroku-account-api-openapi.yml
  format: yaml
  label: Heroku Account API
  slug: heroku-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-account-api-openapi.yml
- filename: heroku-add-ons-api-openapi.yml
  format: yaml
  label: Heroku Add-ons API
  slug: heroku-add-ons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-add-ons-api-openapi.yml
- filename: heroku-apps-api-openapi.yml
  format: yaml
  label: Heroku Apps API
  slug: heroku-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-apps-api-openapi.yml
- filename: heroku-builds-api-openapi.yml
  format: yaml
  label: Heroku Builds API
  slug: heroku-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-builds-api-openapi.yml
- filename: heroku-collaborators-api-openapi.yml
  format: yaml
  label: Heroku Collaborators API
  slug: heroku-collaborators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-collaborators-api-openapi.yml
- filename: heroku-config-vars-api-openapi.yml
  format: yaml
  label: Heroku Config Vars API
  slug: heroku-config-vars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-config-vars-api-openapi.yml
- filename: heroku-domains-api-openapi.yml
  format: yaml
  label: Heroku Domains API
  slug: heroku-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-domains-api-openapi.yml
- filename: heroku-dynos-api-openapi.yml
  format: yaml
  label: Heroku Dynos API
  slug: heroku-dynos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-dynos-api-openapi.yml
- filename: heroku-formation-api-openapi.yml
  format: yaml
  label: Heroku Formation API
  slug: heroku-formation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-formation-api-openapi.yml
- filename: heroku-log-sessions-api-openapi.yml
  format: yaml
  label: Heroku Log Sessions API
  slug: heroku-log-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-log-sessions-api-openapi.yml
- filename: heroku-pipelines-api-openapi.yml
  format: yaml
  label: Heroku Pipelines API
  slug: heroku-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-pipelines-api-openapi.yml
- filename: heroku-regions-api-openapi.yml
  format: yaml
  label: Heroku Regions API
  slug: heroku-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-regions-api-openapi.yml
- filename: heroku-releases-api-openapi.yml
  format: yaml
  label: Heroku Releases API
  slug: heroku-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-releases-api-openapi.yml
- filename: heroku-stacks-api-openapi.yml
  format: yaml
  label: Heroku Stacks API
  slug: heroku-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-stacks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: heroku.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: devcenter.heroku.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 07:02:04 2026 GMT
  host: www.heroku.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: api.heroku.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heroku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heroku, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Heroku
provider_slug: heroku
slug: heroku-domain-security
source_filename: heroku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devcenter.heroku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.heroku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 07:02:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.heroku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: heroku.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/security/heroku-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Deployment
- Cloud Platform
- DevOps
- PaaS
---
