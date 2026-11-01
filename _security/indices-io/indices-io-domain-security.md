---
api_specs:
- filename: indices-io-openapi.json
  format: json
  label: Indices API
  slug: indices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indices-io/openapi/indices-io-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: indices.io
  spf: true
hosts:
- cert_expires: Jan 22 23:23:27 2027 GMT
  host: indices.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Indices Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for indices-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: indices-io
provider_slug: indices-io
slug: indices-io-domain-security
source_filename: indices-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indices.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:23:27 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: indices.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/indices-io/security/indices-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Infrastructure
- Real-time
- Security
---
