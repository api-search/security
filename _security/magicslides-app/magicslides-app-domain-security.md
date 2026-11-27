---
api_specs:
- filename: magicslides-app-presentations-api-openapi.yml
  format: yaml
  label: MagicSlides Presentations API
  slug: magicslides-app-presentations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicslides-app/openapi/magicslides-app-presentations-api-openapi.yml
- filename: magicslides-app-studio-api-openapi.yml
  format: yaml
  label: MagicSlides Studio API
  slug: magicslides-app-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicslides-app/openapi/magicslides-app-studio-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: magicslides.app
  spf: true
hosts:
- cert_expires: Dec 18 20:24:50 2026 GMT
  host: magicslides.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MagicSlides Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MagicSlides, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MagicSlides
provider_slug: magicslides-app
slug: magicslides-app-domain-security
source_filename: magicslides-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magicslides.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 20:24:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: magicslides.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/magicslides-app/security/magicslides-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Presentation
- Automation
- Software-as-a-Service
- Productivity
---
