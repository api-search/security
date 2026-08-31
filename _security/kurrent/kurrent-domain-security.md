---
api_specs:
- filename: kurrent-admin-api-openapi.yml
  format: yaml
  label: Kurrent Admin API
  slug: kurrent-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/openapi/kurrent-admin-api-openapi.yml
- filename: kurrent-gossip-api-openapi.yml
  format: yaml
  label: Kurrent Gossip API
  slug: kurrent-gossip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/openapi/kurrent-gossip-api-openapi.yml
- filename: kurrent-info-api-openapi.yml
  format: yaml
  label: Kurrent Info API
  slug: kurrent-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/openapi/kurrent-info-api-openapi.yml
- filename: kurrent-projections-api-openapi.yml
  format: yaml
  label: Kurrent Projections API
  slug: kurrent-projections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/openapi/kurrent-projections-api-openapi.yml
- filename: kurrent-statistics-api-openapi.yml
  format: yaml
  label: Kurrent Statistics API
  slug: kurrent-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/openapi/kurrent-statistics-api-openapi.yml
- filename: kurrent-streams-api-openapi.yml
  format: yaml
  label: Kurrent Streams API
  slug: kurrent-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/openapi/kurrent-streams-api-openapi.yml
- filename: kurrent-subscriptions-api-openapi.yml
  format: yaml
  label: Kurrent Subscriptions API
  slug: kurrent-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/openapi/kurrent-subscriptions-api-openapi.yml
- filename: kurrent-users-api-openapi.yml
  format: yaml
  label: Kurrent Users API
  slug: kurrent-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/openapi/kurrent-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kurrent.io
  spf: true
hosts:
- cert_expires: Aug 27 16:22:03 2026 GMT
  host: www.kurrent.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 16:09:38 2026 GMT
  host: docs.kurrent.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kurrent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kurrent, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kurrent
provider_slug: kurrent
slug: kurrent-domain-security
source_filename: kurrent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kurrent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 16:22:03 2026 GMT\n  hsts: false\n- host: docs.kurrent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 16:09:38 2026 GMT\n  hsts: false\ndomains:\n- domain: kurrent.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/security/kurrent-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Database
- Event Sourcing
- Event Streaming
- Event Driven Architecture
- CQRS
- Data Infrastructure
- Developer Tools
- Cloud
- Open-Source
- gRPC
- Agentic AI
---
