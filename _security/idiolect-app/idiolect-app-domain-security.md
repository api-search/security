---
api_specs:
- filename: idiolect-app-openapi-generated.yml
  format: yaml
  label: Idiolect AI API
  slug: idiolect-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/idiolect-app/openapi/_ae-authored/idiolect-app-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: idiolect.app
  spf: true
hosts:
- cert_expires: Jan  6 10:34:49 2027 GMT
  host: idiolect.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Idiolect AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Idiolect AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Idiolect AI
provider_slug: idiolect-app
slug: idiolect-app-domain-security
source_filename: idiolect-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: idiolect.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 10:34:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: idiolect.app\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/idiolect-app/security/idiolect-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Writing
- Personalization
- Voice
- Platform
---
