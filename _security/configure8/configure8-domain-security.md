---
api_specs:
- filename: configure8-catalog-entities-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Entities API
  slug: configure8-catalog-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-entities-api-openapi.yml
- filename: configure8-catalog-relations-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Relations API
  slug: configure8-catalog-relations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-relations-api-openapi.yml
- filename: configure8-deployments-api-openapi.yml
  format: yaml
  label: Configure8 Deployments API
  slug: configure8-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-deployments-api-openapi.yml
- filename: configure8-scorecards-api-openapi.yml
  format: yaml
  label: Configure8 Scorecards API
  slug: configure8-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-scorecards-api-openapi.yml
- filename: configure8-users-api-openapi.yml
  format: yaml
  label: Configure8 Users API
  slug: configure8-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: configure8.io
  spf: false
hosts:
- cert_expires: Sep  8 10:09:06 2026 GMT
  host: www.configure8.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: app.configure8.io
  https: false
kind: domain-security
layout: security
method: probed
name: Configure8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Configure8, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Configure8
provider_slug: configure8
slug: configure8-domain-security
source_filename: configure8-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.configure8.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 10:09:06 2026 GMT\n  hsts: false\n- host: app.configure8.io\n  https: false\ndomains:\n- domain: configure8.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/security/configure8-domain-security.yml
summary_line: TLSv1.3
tags:
- Catalog
- Cloud Cost
- Developer Experience
- DevOps
- Internal Developer Portal
- Platform Engineering
- Scorecards
- Self-Service
- Service Catalog
- SRE
---
