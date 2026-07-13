---
api_specs:
- filename: fauna-core-http-api-openapi.yml
  format: yaml
  label: Fauna Core HTTP API
  slug: core-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fauna/refs/heads/main/openapi/fauna-core-http-api-openapi.yml
- filename: fauna-event-streaming-asyncapi.yml
  format: yaml
  label: Fauna Event Streaming API
  slug: event-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fauna/refs/heads/main/asyncapi/fauna-event-streaming-asyncapi.yml
- filename: fauna-graphql-api-openapi.yml
  format: yaml
  label: Fauna GraphQL API
  slug: graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fauna/refs/heads/main/openapi/fauna-graphql-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fauna.com
  spf: true
hosts:
- host: docs.fauna.com
  https: false
- host: db.fauna.com
  https: false
- host: graphql.fauna.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fauna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fauna, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: fauna
provider_slug: fauna
slug: fauna-domain-security
source_filename: fauna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.fauna.com\n  https: false\n- host: db.fauna.com\n  https: false\n- host: graphql.fauna.com\n  https: false\ndomains:\n- domain: fauna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fauna/refs/heads/main/security/fauna-domain-security.yml
summary_line: DMARC
tags: []
---
