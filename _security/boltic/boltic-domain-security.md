---
api_specs:
- filename: boltic-gateway-api-openapi.yml
  format: yaml
  label: Boltic Gateway API
  slug: gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-gateway-api-openapi.yml
- filename: boltic-workflow-api-openapi.yml
  format: yaml
  label: Boltic Workflow API
  slug: workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-workflow-api-openapi.yml
- filename: boltic-tables-api-openapi.yml
  format: yaml
  label: Boltic Tables API
  slug: tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-tables-api-openapi.yml
- filename: boltic-pipes-api-openapi.yml
  format: yaml
  label: Boltic Pipes API
  slug: pipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-pipes-api-openapi.yml
- filename: boltic-streams-api-openapi.yml
  format: yaml
  label: Boltic Streams API
  slug: streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-streams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: boltic.io
  spf: true
hosts:
- cert_expires: Sep 14 12:02:43 2026 GMT
  host: www.boltic.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 09:01:49 2026 GMT
  host: docs.boltic.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 18:12:21 2026 GMT
  host: gateway.boltic.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boltic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boltic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Boltic
provider_slug: boltic
slug: boltic-domain-security
source_filename: boltic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boltic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:02:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.boltic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:01:49 2026 GMT\n  hsts: false\n- host: gateway.boltic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:12:21 2026 GMT\n  hsts: null\ndomains:\n- domain: boltic.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/security/boltic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- DataSync
- Gateways
- NoCode
- Streaming
- Workflows
---
