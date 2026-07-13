---
api_specs:
- filename: trunk-io-openapi.yml
  format: yaml
  label: Trunk Flaky Tests API
  slug: flaky-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trunk-io/refs/heads/main/openapi/trunk-io-openapi.yml
- filename: trunk-io-openapi.yml
  format: yaml
  label: Trunk Merge Queue API
  slug: merge-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trunk-io/refs/heads/main/openapi/trunk-io-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trunk.io
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: trunk.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 16:25:35 2026 GMT
  host: docs.trunk.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api.trunk.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trunk Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trunk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trunk
provider_slug: trunk-io
slug: trunk-io-domain-security
source_filename: trunk-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trunk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.trunk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 16:25:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.trunk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: trunk.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trunk-io/refs/heads/main/security/trunk-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- CI/CD
- Code Quality
- Flaky Tests
- Merge Queue
---
