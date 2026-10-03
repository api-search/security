---
api_specs:
- filename: bnrouter-chat-api-openapi.yml
  format: yaml
  label: bnrouter Chat API
  slug: bnrouter-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnrouter/refs/heads/main/openapi/bnrouter-chat-api-openapi.yml
- filename: bnrouter-images-api-openapi.yml
  format: yaml
  label: bnrouter Images API
  slug: bnrouter-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnrouter/refs/heads/main/openapi/bnrouter-images-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bnrouter.com
  spf: false
hosts:
- cert_expires: Nov 22 17:28:48 2026 GMT
  host: www.bnrouter.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bnrouter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bnrouter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: bnrouter
provider_slug: bnrouter
slug: bnrouter-domain-security
source_filename: bnrouter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bnrouter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 17:28:48 2026 GMT\n  hsts: false\ndomains:\n- domain: bnrouter.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bnrouter/refs/heads/main/security/bnrouter-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Gateways
- Multi-Model
- OpenAI-Compatible
- Developer Tools
---
