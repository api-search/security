---
api_specs:
- filename: shirabe-dev-calendar-api-openapi.yml
  format: yaml
  label: shirabe-dev Calendar API
  slug: shirabe-dev-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shirabe-dev/openapi/shirabe-dev-calendar-api-openapi.yml
- filename: shirabe-dev-hub-api-openapi.yml
  format: yaml
  label: shirabe-dev Hub API
  slug: shirabe-dev-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shirabe-dev/openapi/shirabe-dev-hub-api-openapi.yml
- filename: shirabe-dev-system-api-openapi.yml
  format: yaml
  label: shirabe-dev System API
  slug: shirabe-dev-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shirabe-dev/openapi/shirabe-dev-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shirabe.dev
  spf: true
hosts:
- cert_expires: Jan  5 12:29:20 2027 GMT
  host: shirabe.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shirabe Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for shirabe-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: shirabe-dev
provider_slug: shirabe-dev
slug: shirabe-dev-domain-security
source_filename: shirabe-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shirabe.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 12:29:20 2027 GMT\n  hsts: false\ndomains:\n- domain: shirabe.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/shirabe-dev/security/shirabe-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Platform
- Japanese Data
- Deterministic
- Free Tier
- AI Integration
---
