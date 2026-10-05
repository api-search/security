---
api_specs:
- filename: smartbear-domains-api-openapi.yml
  format: yaml
  label: SmartBear Domains API
  slug: smartbear-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartbear/refs/heads/main/openapi/smartbear-domains-api-openapi.yml
- filename: smartbear-integrations-api-openapi.yml
  format: yaml
  label: SmartBear Integrations API
  slug: smartbear-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartbear/refs/heads/main/openapi/smartbear-integrations-api-openapi.yml
- filename: smartbear-organizations-api-openapi.yml
  format: yaml
  label: SmartBear Organizations API
  slug: smartbear-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartbear/refs/heads/main/openapi/smartbear-organizations-api-openapi.yml
- filename: smartbear-projects-api-openapi.yml
  format: yaml
  label: SmartBear Projects API
  slug: smartbear-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartbear/refs/heads/main/openapi/smartbear-projects-api-openapi.yml
- filename: smartbear-apis-api-openapi.yml
  format: yaml
  label: SmartBear APIs API
  slug: smartbear-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartbear/refs/heads/main/openapi/smartbear-apis-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smartbear.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pactflow.io
  spf: true
hosts:
- cert_expires: Nov 13 07:44:29 2026 GMT
  host: smartbear.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: pactflow.io
  hsts: true
  hsts_max_age: 10368000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  2 21:45:27 2026 GMT
  host: swagger.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Smartbear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmartBear, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SmartBear
provider_slug: smartbear
slug: smartbear-domain-security
source_filename: smartbear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smartbear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 07:44:29 2026 GMT\n  hsts: false\n- host: pactflow.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10368000\n- host: swagger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 21:45:27 2026 GMT\n  hsts: false\ndomains:\n- domain: smartbear.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pactflow.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartbear/refs/heads/main/security/smartbear-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Design
- API Documentation
- API Testing
- Contract Testing
- Developer Tools
- Governance
- Monitoring
- Platform
- Testing
---
