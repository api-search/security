---
api_specs:
- filename: openfga-assertions-api-openapi.yml
  format: yaml
  label: OpenFGA Assertions API
  slug: openfga-assertions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfga/refs/heads/main/openapi/openfga-assertions-api-openapi.yml
- filename: openfga-authorization-models-api-openapi.yml
  format: yaml
  label: OpenFGA Authorization Models API
  slug: openfga-authorization-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfga/refs/heads/main/openapi/openfga-authorization-models-api-openapi.yml
- filename: openfga-authzenservice-api-openapi.yml
  format: yaml
  label: OpenFGA AuthZenService API
  slug: openfga-authzenservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfga/refs/heads/main/openapi/openfga-authzenservice-api-openapi.yml
- filename: openfga-relationship-queries-api-openapi.yml
  format: yaml
  label: OpenFGA Relationship Queries API
  slug: openfga-relationship-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfga/refs/heads/main/openapi/openfga-relationship-queries-api-openapi.yml
- filename: openfga-relationship-tuples-api-openapi.yml
  format: yaml
  label: OpenFGA Relationship Tuples API
  slug: openfga-relationship-tuples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfga/refs/heads/main/openapi/openfga-relationship-tuples-api-openapi.yml
- filename: openfga-stores-api-openapi.yml
  format: yaml
  label: OpenFGA Stores API
  slug: openfga-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfga/refs/heads/main/openapi/openfga-stores-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openfga.dev
  spf: true
hosts:
- cert_expires: Sep  2 18:07:40 2026 GMT
  host: openfga.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openfga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenFGA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenFGA
provider_slug: openfga
slug: openfga-domain-security
source_filename: openfga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openfga.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 18:07:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openfga.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openfga/refs/heads/main/security/openfga-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Access Control
- Authorization
- Cloud Native
- Fine-Grained
- Incubating
- Zanzibar
---
