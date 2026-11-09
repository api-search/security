---
api_specs:
- filename: 0bridge-dev-openapi-generated.yml
  format: yaml
  label: 0bridge API
  slug: 0bridge-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0bridge-dev/openapi/_ae-authored/0bridge-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 0bridge.dev
  spf: true
hosts:
- cert_expires: Dec 24 07:52:22 2026 GMT
  host: 0bridge.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 0Bridge Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 0bridge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 0bridge
provider_slug: 0bridge-dev
slug: 0bridge-dev-domain-security
source_filename: 0bridge-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 0bridge.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 07:52:22 2026 GMT\n  hsts: false\ndomains:\n- domain: 0bridge.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/0bridge-dev/security/0bridge-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- MCP
- Integration
- Team Collaboration
- Productivity
---
