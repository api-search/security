---
api_specs:
- filename: kurrent-kurrentdb-http-api-openapi.yml
  format: yaml
  label: KurrentDB HTTP API
  slug: kurrentdb-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/openapi/kurrent-kurrentdb-http-api-openapi.yml
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
- Open Source
- gRPC
- Agentic AI
---
