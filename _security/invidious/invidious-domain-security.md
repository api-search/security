---
api_specs:
- filename: invidious-invidious-api-api-openapi.yml
  format: yaml
  label: Invidious API
  slug: invidious-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invidious/openapi/invidious-invidious-api-api-openapi.yml
- filename: invidious-openapi-generated.yml
  format: yaml
  label: Invidious API
  slug: invidious-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invidious/openapi/_ae-authored/invidious-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: invidious.io
  spf: true
hosts:
- cert_expires: Dec 10 10:10:17 2026 GMT
  host: invidious.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Invidious Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Invidious, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Invidious
provider_slug: invidious
slug: invidious-domain-security
source_filename: invidious-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: invidious.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 10:10:17 2026 GMT\n  hsts: false\ndomains:\n- domain: invidious.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/invidious/security/invidious-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- video
- open-source
- privacy
- api
- frontend
- youtube
---
