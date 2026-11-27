---
api_specs:
- filename: hostilo-app-files-api-openapi.yml
  format: yaml
  label: Hostilo Files API
  slug: hostilo-app-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostilo-app/openapi/hostilo-app-files-api-openapi.yml
- filename: hostilo-app-sites-api-openapi.yml
  format: yaml
  label: Hostilo Sites API
  slug: hostilo-app-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostilo-app/openapi/hostilo-app-sites-api-openapi.yml
- filename: hostilo-app-statistics-api-openapi.yml
  format: yaml
  label: Hostilo Statistics API
  slug: hostilo-app-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostilo-app/openapi/hostilo-app-statistics-api-openapi.yml
- filename: hostilo-app-templates-api-openapi.yml
  format: yaml
  label: Hostilo Templates API
  slug: hostilo-app-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostilo-app/openapi/hostilo-app-templates-api-openapi.yml
- filename: hostilo-app-versions-api-openapi.yml
  format: yaml
  label: Hostilo Versions API
  slug: hostilo-app-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostilo-app/openapi/hostilo-app-versions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hostilo.app
  spf: true
hosts:
- cert_expires: Dec 13 23:26:18 2026 GMT
  host: hostilo.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hostilo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hostilo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hostilo
provider_slug: hostilo-app
slug: hostilo-app-domain-security
source_filename: hostilo-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hostilo.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:26:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hostilo.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hostilo-app/security/hostilo-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hosting
- Artificial Intelligence
- Free
- Static
---
