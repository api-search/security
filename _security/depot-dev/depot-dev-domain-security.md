---
api_specs:
- filename: depot-dev-buildkitservice-api-openapi.yml
  format: yaml
  label: Depot BuildKitService API
  slug: depot-dev-buildkitservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/openapi/depot-dev-buildkitservice-api-openapi.yml
- filename: depot-dev-buildservice-api-openapi.yml
  format: yaml
  label: Depot BuildService API
  slug: depot-dev-buildservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/openapi/depot-dev-buildservice-api-openapi.yml
- filename: depot-dev-projectservice-api-openapi.yml
  format: yaml
  label: Depot ProjectService API
  slug: depot-dev-projectservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/openapi/depot-dev-projectservice-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: depot.dev
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: depot.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.depot.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Depot Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Depot, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Depot
provider_slug: depot-dev
slug: depot-dev-domain-security
source_filename: depot-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: depot.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\n- host: api.depot.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: depot.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/security/depot-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Container Builds
- Docker
- BuildKit
- Remote Cache
- CI/CD
- GitHub Actions
---
