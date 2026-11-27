---
api_specs:
- filename: findlocal-events-api-openapi.yml
  format: yaml
  label: FindLocal Events API
  slug: findlocal-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findlocal/openapi/findlocal-events-api-openapi.yml
- filename: findlocal-venues-api-openapi.yml
  format: yaml
  label: FindLocal Venues API
  slug: findlocal-venues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findlocal/openapi/findlocal-venues-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: findlocal.community
  spf: true
hosts:
- cert_expires: Feb  1 01:10:48 2027 GMT
  host: findlocal.community
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FindLocal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FindLocal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FindLocal
provider_slug: findlocal
slug: findlocal-domain-security
source_filename: findlocal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: findlocal.community\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 01:10:48 2027 GMT\n  hsts: false\ndomains:\n- domain: findlocal.community\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/findlocal/security/findlocal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Event
- Hyperlocal
- Community
- Data
- Open Data
---
