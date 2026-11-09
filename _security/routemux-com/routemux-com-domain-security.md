---
api_specs:
- filename: routemux-com-chat-completions-api-openapi.yml
  format: yaml
  label: RouteMux Chat Completions API
  slug: routemux-com-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/routemux-com/openapi/routemux-com-chat-completions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: routemux.com
  spf: true
hosts:
- cert_expires: Dec 18 13:47:57 2026 GMT
  host: routemux.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Routemux Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RouteMux, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: RouteMux
provider_slug: routemux-com
slug: routemux-com-domain-security
source_filename: routemux-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: routemux.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 13:47:57 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: routemux.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/routemux-com/security/routemux-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Gateways
- Multi-Model
- Unified API
- Company
---
