---
api_specs:
- filename: aft-page-api-openapi.json
  format: json
  label: aft.page API API
  slug: aft-page-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aft-page/openapi/_original/aft-page-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aft.page
  spf: true
hosts:
- cert_expires: Dec 22 16:49:31 2026 GMT
  host: aft.page
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aft Page Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aft.page, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: aft.page
provider_slug: aft-page
slug: aft-page-domain-security
source_filename: aft-page-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aft.page\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 16:49:31 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: aft.page\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aft-page/security/aft-page-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Hosting
- CLI
- Deployment
- Low‑friction
---
