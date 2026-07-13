---
api_specs:
- filename: upwork-graphql-api-openapi.yml
  format: yaml
  label: Upwork GraphQL API
  slug: graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/openapi/upwork-graphql-api-openapi.yml
- filename: upwork-rest-api-openapi.yml
  format: yaml
  label: Upwork REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/openapi/upwork-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: upwork.com
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: www.upwork.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: api.upwork.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: developers.upwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upwork, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Upwork
provider_slug: upwork
slug: upwork-domain-security
source_filename: upwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.upwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\n- host: api.upwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\n- host: developers.upwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: upwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/security/upwork-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Freelancing
- Jobs
- Talent
- Marketplace
- Contracts
- Hiring
---
