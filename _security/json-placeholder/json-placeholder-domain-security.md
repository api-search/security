---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: JSONPlaceholder API
  slug: json-placeholder-api
  spec_type: OpenAPI
  url: https://github.com/sebastienlevert/jsonplaceholder-api/blob/main/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: typicode.com
  spf: false
hosts:
- cert_expires: Aug 29 22:44:15 2026 GMT
  host: jsonplaceholder.typicode.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Json Placeholder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JSONPlaceholder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: JSONPlaceholder
provider_slug: json-placeholder
slug: json-placeholder-domain-security
source_filename: json-placeholder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jsonplaceholder.typicode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 22:44:15 2026 GMT\n  hsts: false\ndomains:\n- domain: typicode.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/json-placeholder/refs/heads/main/security/json-placeholder-domain-security.yml
summary_line: TLSv1.3
tags:
- Fake API
- Testing
- Prototyping
- Mock Data
- REST
- Open Source
---
