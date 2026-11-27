---
api_specs:
- filename: featury-app-openapi-generated.yml
  format: yaml
  label: featury API
  slug: featury-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/featury-app/openapi/_ae-authored/featury-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: featury.app
  spf: true
hosts:
- cert_expires: Jan 21 22:57:50 2027 GMT
  host: featury.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: featury Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for featury, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: featury
provider_slug: featury-app
slug: featury-app-domain-security
source_filename: featury-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: featury.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 22:57:50 2027 GMT\n  hsts: false\ndomains:\n- domain: featury.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/featury-app/security/featury-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Changelog
- Automation
- Developer Tools
- Open Source
---
