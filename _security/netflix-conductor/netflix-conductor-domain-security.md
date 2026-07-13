---
api_specs:
- filename: conductor-api.yml
  format: yaml
  label: Netflix Conductor
  slug: netflix-conductor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netflix-conductor/refs/heads/main/openapi/conductor-api.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: conductor-oss.org
  spf: false
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: conductor-oss.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netflix Conductor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netflix Conductor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Netflix Conductor
provider_slug: netflix-conductor
slug: netflix-conductor-domain-security
source_filename: netflix-conductor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conductor-oss.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: conductor-oss.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netflix-conductor/refs/heads/main/security/netflix-conductor-domain-security.yml
summary_line: TLSv1.3
tags:
- Event-Driven
- Microservices
- Netflix
- Open Source
- Orchestration
- Workflows
---
