---
api_specs:
- filename: octri-dev-openapi-generated.yml
  format: yaml
  label: Octri API
  slug: octri-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octri-dev/openapi/_ae-authored/octri-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: octri.dev
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: acme.com
  spf: false
hosts:
- cert_expires: Nov 29 20:21:28 2026 GMT
  host: octri.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.acme.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Octri Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octri, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Octri
provider_slug: octri-dev
slug: octri-dev-domain-security
source_filename: octri-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: octri.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 20:21:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.acme.com\n  https: false\ndomains:\n- domain: octri.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: acme.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/octri-dev/security/octri-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API
- Documentation
- SDK
- Monitoring
- MCP
---
