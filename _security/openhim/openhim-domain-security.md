---
api_specs:
- filename: openhim-openapi-generated.yml
  format: yaml
  label: OpenHIM API
  slug: openhim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openhim/openapi/_ae-authored/openhim-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openhim.org
  spf: false
hosts:
- cert_expires: Jan 24 19:36:57 2027 GMT
  host: openhim.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenHIM Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenHIM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenHIM
provider_slug: openhim
slug: openhim-domain-security
source_filename: openhim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openhim.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 19:36:57 2027 GMT\n  hsts: false\ndomains:\n- domain: openhim.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/openhim/security/openhim-domain-security.yml
summary_line: TLSv1.3
tags:
- Health
- Integration
- Middleware
- Open Source
---
