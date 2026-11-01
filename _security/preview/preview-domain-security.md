---
api_specs:
- filename: preview-openapi-generated.yml
  format: yaml
  label: Preview API
  slug: preview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preview/openapi/_ae-authored/preview-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: preview.io
  spf: true
hosts:
- cert_expires: Jan  3 09:22:16 2027 GMT
  host: preview.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Preview Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Preview, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Preview
provider_slug: preview
slug: preview-domain-security
source_filename: preview-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: preview.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 09:22:16 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: preview.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/preview/security/preview-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Video
- Collaboration
- Production
---
