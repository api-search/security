---
api_specs:
- filename: hooklayer-dev-openapi-generated.yml
  format: yaml
  label: hooklayer-dev API
  slug: hooklayer-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hooklayer-dev/openapi/_ae-authored/hooklayer-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hooklayer.dev
  spf: false
hosts:
- cert_expires: Dec 11 18:52:02 2026 GMT
  host: hooklayer.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hooklayer Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hooklayer-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: hooklayer-dev
provider_slug: hooklayer-dev
slug: hooklayer-dev-domain-security
source_filename: hooklayer-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hooklayer.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 18:52:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hooklayer.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hooklayer-dev/security/hooklayer-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- MCP
- AI
- Video
- Marketing
- Analytics
- Content
---
