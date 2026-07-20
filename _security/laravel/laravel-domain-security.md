---
api_specs:
- filename: laravel-forge-openapi.json
  format: json
  label: Laravel Forge API
  slug: forge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laravel/refs/heads/main/openapi/laravel-forge-openapi.json
- filename: laravel-cloud-openapi.json
  format: json
  label: Laravel Cloud API
  slug: cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laravel/refs/heads/main/openapi/laravel-cloud-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: laravel.com
  spf: true
hosts:
- cert_expires: Sep  9 18:01:51 2026 GMT
  host: laravel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 17:09:36 2026 GMT
  host: forge.laravel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 12:13:19 2026 GMT
  host: cloud.laravel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Laravel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laravel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Laravel
provider_slug: laravel
slug: laravel-domain-security
source_filename: laravel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laravel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 18:01:51 2026 GMT\n  hsts: false\n- host: forge.laravel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:09:36 2026 GMT\n  hsts: false\n- host: cloud.laravel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 12:13:19 2026 GMT\n  hsts: false\ndomains:\n- domain: laravel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laravel/refs/heads/main/security/laravel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud Saas
- PHP
- Developer Tools
- Platform as a Service
- Deployment
- Server Management
- Application Hosting
- Infrastructure
- Frameworks
- Monitoring
---
