---
api_specs:
- filename: immich-openapi-generated.yml
  format: yaml
  label: Immich API
  slug: immich-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immich/openapi/_ae-authored/immich-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: immich.app
  spf: true
hosts:
- cert_expires: Dec 14 08:43:44 2026 GMT
  host: immich.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Immich Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Immich, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Immich
provider_slug: immich
slug: immich-domain-security
source_filename: immich-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: immich.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 08:43:44 2026 GMT\n  hsts: false\ndomains:\n- domain: immich.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/immich/security/immich-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Self-Hosted
- Photo Management
- Video Management
- Privacy
- Open Source
---
