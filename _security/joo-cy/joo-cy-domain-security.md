---
api_specs:
- filename: joo-cy-openapi-generated.yml
  format: yaml
  label: Joocy API
  slug: joo-cy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joo-cy/openapi/_ae-authored/joo-cy-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joo.cy
  spf: true
hosts:
- cert_expires: Jan 11 22:45:56 2027 GMT
  host: joo.cy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Joocy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joocy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Joocy
provider_slug: joo-cy
slug: joo-cy-domain-security
source_filename: joo-cy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joo.cy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 22:45:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: joo.cy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/joo-cy/security/joo-cy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Interactive
- Presentation
- Live Polling
- Audience Engagement
- Artificial Intelligence
---
