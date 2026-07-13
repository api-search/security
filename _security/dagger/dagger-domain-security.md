---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dagger.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: daggerverse.dev
  spf: false
hosts:
- cert_expires: Sep 10 18:43:55 2026 GMT
  host: dagger.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 21:23:45 2026 GMT
  host: docs.dagger.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: daggerverse.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dagger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dagger, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dagger
provider_slug: dagger
slug: dagger-domain-security
source_filename: dagger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dagger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 18:43:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dagger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 21:23:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: daggerverse.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: dagger.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: daggerverse.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dagger/refs/heads/main/security/dagger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Build Automation
- BuildKit
- CI/CD
- Containers
- DAG
- Daggerverse
- DevOps
- GraphQL
- Modules
- OCI
- Open Source
- Pipelines
- Programmable Pipelines
- SDKs
---
