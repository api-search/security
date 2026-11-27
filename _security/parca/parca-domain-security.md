---
api_specs:
- filename: parca-openapi-generated.yml
  format: yaml
  label: Parca API
  slug: parca-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parca/openapi/_ae-authored/parca-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: parca.dev
  spf: true
hosts:
- cert_expires: Dec 29 11:00:16 2026 GMT
  host: parca.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Parca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parca, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Parca
provider_slug: parca
slug: parca-domain-security
source_filename: parca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parca.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 11:00:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: parca.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/parca/security/parca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Source
- Profiling
- eBPF
- Cloud-Native
- Observability
- Performance
---
