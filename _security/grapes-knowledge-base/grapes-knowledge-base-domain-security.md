---
api_specs:
- filename: grapes-knowledge-base-openapi.yml
  format: yaml
  label: Grapes API
  slug: grapes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grapes-knowledge-base/refs/heads/main/openapi/grapes-knowledge-base-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: data-grapes.com
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: docs.data-grapes.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: api.data-grapes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grapes Knowledge Base Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grapes Knowledge Base, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Grapes Knowledge Base
provider_slug: grapes-knowledge-base
slug: grapes-knowledge-base-domain-security
source_filename: grapes-knowledge-base-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.data-grapes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: api.data-grapes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: data-grapes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grapes-knowledge-base/refs/heads/main/security/grapes-knowledge-base-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Knowledge Management
- Knowledge Base
- Data Management
- Automation
- HATEOAS
---
