---
api_specs:
- filename: jsonplaceholder-openapi.yml
  format: yaml
  label: JSONPlaceholder REST API
  slug: jsonplaceholder-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jsonplaceholder/refs/heads/main/openapi/jsonplaceholder-openapi.yml
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
name: Jsonplaceholder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JSONPlaceholder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: JSONPlaceholder
provider_slug: jsonplaceholder
slug: jsonplaceholder-domain-security
source_filename: jsonplaceholder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jsonplaceholder.typicode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 22:44:15 2026 GMT\n  hsts: false\ndomains:\n- domain: typicode.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jsonplaceholder/refs/heads/main/security/jsonplaceholder-domain-security.yml
summary_line: TLSv1.3
tags:
- Development
- Testing
- Prototyping
- Fake API
- Open Source
- REST
---
