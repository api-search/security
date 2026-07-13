---
api_specs:
- filename: noun-project-openapi.yml
  format: yaml
  label: Noun Project API V2
  slug: noun-project-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noun-project/refs/heads/main/openapi/noun-project-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thenounproject.com
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: thenounproject.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: api.thenounproject.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noun Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noun Project, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Noun Project
provider_slug: noun-project
slug: noun-project-domain-security
source_filename: noun-project-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thenounproject.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: false\n- host: api.thenounproject.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: thenounproject.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noun-project/refs/heads/main/security/noun-project-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Art And Design
- Icons
- SVG
- Visual Language
- Design Assets
- Public APIs
---
