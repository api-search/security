---
api_specs:
- filename: openclip-app-openapi-generated.yml
  format: yaml
  label: OpenClip API
  slug: openclip-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openclip-app/openapi/_ae-authored/openclip-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openclip.app
  spf: true
hosts:
- cert_expires: Jan 21 16:12:58 2027 GMT
  host: openclip.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenClip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenClip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: OpenClip
provider_slug: openclip-app
slug: openclip-app-domain-security
source_filename: openclip-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openclip.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 16:12:58 2027 GMT\n  hsts: false\ndomains:\n- domain: openclip.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/openclip-app/security/openclip-app-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Video Editing
- Content Creation
- Social Media
---
