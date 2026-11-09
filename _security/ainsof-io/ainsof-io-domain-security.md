---
api_specs:
- filename: ainsof-io-openapi-generated.yml
  format: yaml
  label: AINSOF API
  slug: ainsof-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainsof-io/openapi/_ae-authored/ainsof-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ainsof.io
  spf: true
hosts:
- cert_expires: Dec 28 06:33:50 2026 GMT
  host: ainsof.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ainsof Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AINSOF, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: AINSOF
provider_slug: ainsof-io
slug: ainsof-io-domain-security
source_filename: ainsof-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ainsof.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 06:33:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ainsof.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ainsof-io/security/ainsof-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Music
- Artificial Intelligence
- Licensing
- Media
---
