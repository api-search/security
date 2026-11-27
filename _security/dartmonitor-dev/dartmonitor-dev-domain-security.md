---
api_specs:
- filename: dartmonitor-dev-openapi-generated.yml
  format: yaml
  label: dartmonitor-dev API
  slug: dartmonitor-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dartmonitor-dev/openapi/_ae-authored/dartmonitor-dev-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dartmonitor.dev
  spf: true
hosts:
- cert_expires: Jan 20 06:13:48 2027 GMT
  host: dartmonitor.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: dartmonitor-dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dartmonitor-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: dartmonitor-dev
provider_slug: dartmonitor-dev
slug: dartmonitor-dev-domain-security
source_filename: dartmonitor-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dartmonitor.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 06:13:48 2027 GMT\n  hsts: false\ndomains:\n- domain: dartmonitor.dev\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dartmonitor-dev/security/dartmonitor-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Flutter
- Dart
- CI
- Email Alerts
---
