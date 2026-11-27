---
api_specs:
- filename: muse-space-read-api-openapi.yml
  format: yaml
  label: Muse Read API
  slug: muse-space-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muse-space/openapi/muse-space-read-api-openapi.yml
- filename: muse-space-write-api-openapi.yml
  format: yaml
  label: Muse Write API
  slug: muse-space-write-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muse-space/openapi/muse-space-write-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: muse.space
  spf: true
hosts:
- cert_expires: Dec 21 22:39:02 2026 GMT
  host: muse.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Muse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Muse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Muse
provider_slug: muse-space
slug: muse-space-domain-security
source_filename: muse-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: muse.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 22:39:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: muse.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/muse-space/security/muse-space-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Calendar
- Email
- Privacy
---
