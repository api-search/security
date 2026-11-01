---
api_specs:
- filename: beszel-beszel-api-api-openapi.yml
  format: yaml
  label: Beszel API
  slug: beszel-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beszel/openapi/beszel-beszel-api-api-openapi.yml
- filename: beszel-openapi-generated.yml
  format: yaml
  label: Beszel API
  slug: beszel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beszel/openapi/_ae-authored/beszel-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: beszel.dev
  spf: true
hosts:
- cert_expires: Dec 28 04:08:15 2026 GMT
  host: beszel.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beszel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beszel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Beszel
provider_slug: beszel
slug: beszel-domain-security
source_filename: beszel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beszel.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 04:08:15 2026 GMT\n  hsts: false\ndomains:\n- domain: beszel.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/beszel/security/beszel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Server Monitoring
- Docker
- Podman
- Alerts
- Multi‑user
- OAuth
- Backup
- REST API
---
