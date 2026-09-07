---
api_specs:
- filename: anew-openapi.json
  format: json
  label: anew Write/Read API
  slug: anew-writeread-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anew/refs/heads/main/openapi/anew-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: anew.page
  spf: false
hosts:
- cert_expires: Nov  1 10:30:08 2026 GMT
  host: anew.page
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anew Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for anew, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: anew
provider_slug: anew
slug: anew-domain-security
source_filename: anew-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anew.page\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 10:30:08 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: anew.page\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anew/refs/heads/main/security/anew-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- html
- webpage
- website
- url
- encode
- share
- web-publishing
- developer-tools
- mcp
- a2a
- ai-agent-tooling
- llms-txt
- agents-txt
- agent-skills
- webmcp
- openapi
- stateless
- immutable
- no-auth
- static-site
- url-encoding
---
