---
api_specs:
- filename: openapi.json
  format: json
  label: Hex.pm API
  slug: hexpm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: hex.pm
  spf: true
hosts:
- cert_expires: Aug 29 00:20:27 2026 GMT
  host: hex.pm
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hex Pm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hex.pm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hex.pm
provider_slug: hex-pm
slug: hex-pm-domain-security
source_filename: hex-pm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hex.pm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:20:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hex.pm\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/security/hex-pm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Package Registry
- Erlang
- Elixir
- Gleam
- BEAM
- Open Source
- Package Manager
---
