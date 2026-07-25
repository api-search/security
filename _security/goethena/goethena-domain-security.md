---
api_specs:
- filename: goethena-learner-training-campaigns-api-openapi.yml
  format: yaml
  label: Goethena Learner Training Campaigns API
  slug: goethena-learner-training-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goethena/refs/heads/main/openapi/goethena-learner-training-campaigns-api-openapi.yml
- filename: goethena-learner-training-modules-api-openapi.yml
  format: yaml
  label: Goethena Learner Training Modules API
  slug: goethena-learner-training-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goethena/refs/heads/main/openapi/goethena-learner-training-modules-api-openapi.yml
- filename: goethena-learners-api-openapi.yml
  format: yaml
  label: Goethena Learners API
  slug: goethena-learners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goethena/refs/heads/main/openapi/goethena-learners-api-openapi.yml
- filename: goethena-training-campaigns-api-openapi.yml
  format: yaml
  label: Goethena Training Campaigns API
  slug: goethena-training-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goethena/refs/heads/main/openapi/goethena-training-campaigns-api-openapi.yml
- filename: goethena-webhooks-api-openapi.yml
  format: yaml
  label: Goethena Webhooks API
  slug: goethena-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goethena/refs/heads/main/openapi/goethena-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: goethena.com
  spf: true
hosts:
- cert_expires: Sep  4 19:34:29 2026 GMT
  host: goethena.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.goethena.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goethena Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goethena, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Goethena
provider_slug: goethena
slug: goethena-domain-security
source_filename: goethena-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goethena.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 19:34:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.goethena.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: goethena.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goethena/refs/heads/main/security/goethena-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Compliance
- Training
- Human Resources
- Ethics
- Learning Management
- AI Agents
- Governance
- Workforce
---
