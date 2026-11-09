---
api_specs:
- filename: ceki-me-openapi-generated.yml
  format: yaml
  label: Ceki.me API
  slug: ceki-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ceki-me/openapi/_ae-authored/ceki-me-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ceki.me
  spf: true
hosts:
- cert_expires: Jan 27 02:54:27 2027 GMT
  host: ceki.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ceki Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ceki.me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ceki.me
provider_slug: ceki-me
slug: ceki-me-domain-security
source_filename: ceki-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ceki.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 02:54:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ceki.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ceki-me/security/ceki-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Productivity
- Marketplace
- Collaboration
- Time Tracking
---
