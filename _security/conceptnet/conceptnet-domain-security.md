---
api_specs:
- filename: openapi.yml
  format: yaml
  label: ConceptNet REST API
  slug: conceptnet-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conceptnet/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: conceptnet.io
  spf: false
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: conceptnet.io
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: api.conceptnet.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Conceptnet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConceptNet, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ConceptNet
provider_slug: conceptnet
slug: conceptnet-domain-security
source_filename: conceptnet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conceptnet.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n- host: api.conceptnet.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: conceptnet.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conceptnet/refs/heads/main/security/conceptnet-domain-security.yml
summary_line: TLSv1.2
tags:
- Knowledge Graph
- NLP
- Semantic Web
- Common Sense
- Multilingual
- Word Embeddings
- Linked Data
- Open Data
---
