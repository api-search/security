---
api_specs:
- filename: danseici-fr-events-api-openapi.yml
  format: yaml
  label: Danse Ici Events API
  slug: danseici-fr-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/danseici-fr/openapi/danseici-fr-events-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: danseici.fr
  spf: true
hosts:
- cert_expires: Dec 23 14:51:46 2026 GMT
  host: danseici.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Danse Ici Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Danse Ici, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Danse Ici
provider_slug: danseici-fr
slug: danseici-fr-domain-security
source_filename: danseici-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: danseici.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 14:51:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: danseici.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/danseici-fr/security/danseici-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Dance
- Event
- Paris
- Community
- Platform
---
