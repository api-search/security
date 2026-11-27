---
api_specs:
- filename: frankki-app-openapi-generated.yml
  format: yaml
  label: FrankKi API
  slug: frankki-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frankki-app/openapi/_ae-authored/frankki-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: frankki.app
  spf: false
hosts:
- cert_expires: Feb  2 04:29:06 2027 GMT
  host: frankki.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FrankKi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FrankKi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FrankKi
provider_slug: frankki-app
slug: frankki-app-domain-security
source_filename: frankki-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frankki.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 04:29:06 2027 GMT\n  hsts: false\ndomains:\n- domain: frankki.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/frankki-app/security/frankki-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Automation
- Messaging
- Software-as-a-Service
---
