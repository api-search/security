---
api_specs:
- filename: customeros-customerbase-openapi.yml
  format: yaml
  label: CustomerOS REST API
  slug: customeros-customerbase-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-customerbase-openapi.yml
- filename: customeros-flow-api-openapi.yml
  format: yaml
  label: CustomerOS Flow API
  slug: customeros-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-flow-api-openapi.yml
- filename: customeros-graphql-api-openapi.yml
  format: yaml
  label: CustomerOS GraphQL API
  slug: customeros-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-graphql-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: customeros.ai
  spf: true
hosts:
- cert_expires: Oct  9 00:39:16 2026 GMT
  host: customeros.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 07:46:47 2026 GMT
  host: docs.customeros.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.customeros.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Customeros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CustomerOS, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CustomerOS
provider_slug: customeros
slug: customeros-domain-security
source_filename: customeros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: customeros.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 00:39:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.customeros.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 07:46:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.customeros.ai\n  https: false\ndomains:\n- domain: customeros.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/security/customeros-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CRM
- Revenue
- Go-To-Market
- Lead Intelligence
- Visitor Identification
- Attribution
- Email Verification
- Enrichment
- GraphQL
- Open-Source
---
