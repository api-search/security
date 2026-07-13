---
api_specs:
- filename: trino-client-api-openapi.yml
  format: yaml
  label: Trino Client REST API
  slug: trino-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trino/refs/heads/main/openapi/trino-client-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trino.io
  spf: true
hosts:
- cert_expires: Sep 16 05:44:43 2026 GMT
  host: trino.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trino Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trino, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Trino
provider_slug: trino
slug: trino-domain-security
source_filename: trino-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trino.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 05:44:43 2026 GMT\n  hsts: false\ndomains:\n- domain: trino.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trino/refs/heads/main/security/trino-domain-security.yml
summary_line: TLSv1.3
tags:
- Analytics
- Big Data
- Distributed SQL
- MySQL
- NoSQL
- Queries
- SQL
---
