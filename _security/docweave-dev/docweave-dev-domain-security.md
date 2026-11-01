---
api_specs:
- filename: docweave-dev-openapi-generated.yml
  format: yaml
  label: docweave-dev API
  slug: docweave-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docweave-dev/openapi/_ae-authored/docweave-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: docweave.dev
  spf: true
hosts:
- cert_expires: Dec 15 14:45:52 2026 GMT
  host: docweave.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docweave Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for docweave-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: docweave-dev
provider_slug: docweave-dev
slug: docweave-dev-domain-security
source_filename: docweave-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docweave.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 14:45:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: docweave.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/docweave-dev/security/docweave-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- PDF
- Generation
- API
- AI
- Developers
---
