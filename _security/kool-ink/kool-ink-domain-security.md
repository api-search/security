---
api_specs:
- filename: kool-ink-openapi-generated.yml
  format: yaml
  label: KooLink API
  slug: kool-ink-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kool-ink/openapi/_ae-authored/kool-ink-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kool.ink
  spf: true
hosts:
- cert_expires: Dec 31 08:40:57 2026 GMT
  host: kool.ink
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KooLink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KooLink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: KooLink
provider_slug: kool-ink
slug: kool-ink-domain-security
source_filename: kool-ink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kool.ink\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 08:40:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kool.ink\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kool-ink/security/kool-ink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- URL Shortening
- Free
- Creator Earnings
---
