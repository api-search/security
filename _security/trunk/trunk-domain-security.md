---
api_specs:
- filename: trunk-openapi.yml
  format: yaml
  label: Trunk Flaky Tests API
  slug: flaky-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trunk/refs/heads/main/openapi/trunk-openapi.yml
- filename: trunk-openapi.yml
  format: yaml
  label: Trunk Merge Queue API
  slug: merge-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trunk/refs/heads/main/openapi/trunk-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trunk.io
  spf: true
hosts:
- host: trunk.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: docs.trunk.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.trunk.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trunk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trunk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trunk
provider_slug: trunk
slug: trunk-domain-security
source_filename: trunk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trunk.io\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.trunk.io\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.trunk.io\n  https: true\n  tls_version: TLSv1.3\n  hsts: null\ndomains:\n- domain: trunk.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trunk/refs/heads/main/security/trunk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- CI/CD
- Code Quality
- Flaky Tests
- Merge Queue
- Test Analytics
- Static Analysis
- Webhooks
---
