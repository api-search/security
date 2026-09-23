---
api_specs:
- filename: openhandle-openapi.yml
  format: yaml
  label: Openhandle API
  slug: openhandle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openhandle/refs/heads/main/openapi/openhandle-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openhandle.dev
  spf: true
hosts:
- cert_expires: Nov  1 17:41:09 2026 GMT
  host: openhandle.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 13:26:52 2026 GMT
  host: api.openhandle.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Openhandle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Openhandle, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Openhandle
provider_slug: openhandle
slug: openhandle-domain-security
source_filename: openhandle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openhandle.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 17:41:09 2026 GMT\n  hsts: false\n- host: api.openhandle.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 13:26:52 2026 GMT\n  hsts: null\ndomains:\n- domain: openhandle.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openhandle/refs/heads/main/security/openhandle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social Data
- Instagram
- TikTok
- twitter
- Reddit
- Public Data
- social-media-api
- MCP
- creator-analytics
- Social Listening
---
