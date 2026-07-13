---
api_specs:
- filename: bazel-central-registry-openapi.yml
  format: yaml
  label: Bazel Central Registry API
  slug: bazel-central-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazel-build/refs/heads/main/openapi/bazel-central-registry-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bazel.build
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: bazel.build
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 12:30:19 2026 GMT
  host: registry.bazel.build
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 16:18:35 2026 GMT
  host: bcr.bazel.build
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bazel Build Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bazel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bazel
provider_slug: bazel-build
slug: bazel-build-domain-security
source_filename: bazel-build-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bazel.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: registry.bazel.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 12:30:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: bcr.bazel.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 16:18:35 2026 GMT\n  hsts: false\ndomains:\n- domain: bazel.build\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bazel-build/refs/heads/main/security/bazel-build-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Build Systems
- Build Tool
- Bzlmod
- CI/CD
- Developer Tools
- Hermetic Builds
- Monorepo
- Open Source
- Remote Execution
- Starlark
---
