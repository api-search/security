---
api_specs:
- filename: opslevel-openapi.yml
  format: yaml
  label: OpsLevel GraphQL API
  slug: graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opslevel/refs/heads/main/openapi/opslevel-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opslevel.com
  spf: true
hosts:
- cert_expires: Aug 16 11:04:13 2026 GMT
  host: www.opslevel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 18:32:40 2026 GMT
  host: docs.opslevel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: api.opslevel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opslevel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpsLevel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OpsLevel
provider_slug: opslevel
slug: opslevel-domain-security
source_filename: opslevel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opslevel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 11:04:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.opslevel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 18:32:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.opslevel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: opslevel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opslevel/refs/heads/main/security/opslevel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Portal
- DevOps
- Experience
- Internal Developer Portal
- Microservices
- Platform Engineering
- Service Catalog
- Service Maturity
---
