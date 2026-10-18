---
api_specs:
- filename: cloudhealthsystems-aws-accounts-api-openapi.yml
  format: yaml
  label: Cloudhealthsystems Aws Accounts API
  slug: cloudhealthsystems-aws-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealthsystems/refs/heads/main/openapi/cloudhealthsystems-aws-accounts-api-openapi.yml
- filename: cloudhealthsystems-cloudhealthsystems-api-api-openapi.yml
  format: yaml
  label: Cloudhealthsystems Cloudhealthsystems API
  slug: cloudhealthsystems-cloudhealthsystems-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealthsystems/refs/heads/main/openapi/cloudhealthsystems-cloudhealthsystems-api-api-openapi.yml
- filename: cloudhealthsystems-olap-reports-api-openapi.yml
  format: yaml
  label: Cloudhealthsystems Olap Reports API
  slug: cloudhealthsystems-olap-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealthsystems/refs/heads/main/openapi/cloudhealthsystems-olap-reports-api-openapi.yml
- filename: cloudhealthsystems-perspective-schemas-api-openapi.yml
  format: yaml
  label: Cloudhealthsystems Perspective Schemas API
  slug: cloudhealthsystems-perspective-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealthsystems/refs/heads/main/openapi/cloudhealthsystems-perspective-schemas-api-openapi.yml
- filename: cloudhealthsystems-rest-api-openapi.yml
  format: yaml
  label: Cloudhealthsystems Rest API
  slug: cloudhealthsystems-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealthsystems/refs/heads/main/openapi/cloudhealthsystems-rest-api-openapi.yml
- filename: cloudhealthsystems-sso-api-openapi.yml
  format: yaml
  label: Cloudhealthsystems SSO API
  slug: cloudhealthsystems-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealthsystems/refs/heads/main/openapi/cloudhealthsystems-sso-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cloudhealthtech.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: apps.cloudhealthtech.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloudhealthsystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudhealthsystems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cloudhealthsystems
provider_slug: cloudhealthsystems
slug: cloudhealthsystems-domain-security
source_filename: cloudhealthsystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apps.cloudhealthtech.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cloudhealthtech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudhealthsystems/refs/heads/main/security/cloudhealthsystems-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Cloud
- Financial Management
- Multi-Cloud
- Cost Optimization
- Governance
---
