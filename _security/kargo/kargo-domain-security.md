---
api_specs:
- filename: kargo-document-intake-openapi.yml
  format: yaml
  label: Kargo Document Intake API
  slug: kargo-document-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kargo/refs/heads/main/openapi/kargo-document-intake-openapi.yml
- filename: kargo-public-graphql.postman_collection.json
  format: json
  label: Kargo Public GraphQL API
  slug: kargo-public-graphql-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/kargo/refs/heads/main/postman/kargo-public-graphql.postman_collection.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kargo.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: kargo.zone
  spf: true
hosts:
- cert_expires: Oct 22 17:25:23 2026 GMT
  host: www.kargo.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 13:06:01 2026 GMT
  host: docs.kargo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.kargo.zone
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kargo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kargo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kargo
provider_slug: kargo
slug: kargo-domain-security
source_filename: kargo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kargo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 17:25:23 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.kargo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:06:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.kargo.zone\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kargo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: kargo.zone\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kargo/refs/heads/main/security/kargo-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Logistics
- Supply Chain
- Warehouse
- Computer Vision
- Artificial Intelligence
- Shipping
- Inventory
- Industrial Automation
- Freight
- GraphQL
- Webhooks
---
