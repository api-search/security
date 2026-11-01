---
api_specs:
- filename: orchesty-2.0-openapi-generated.yml
  format: yaml
  label: Orchesty.io 2.0 API
  slug: 2.0-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orchesty/openapi/_ae-authored/orchesty-2.0-openapi-generated.yml
- filename: orchesty-3.0-openapi-generated.yml
  format: yaml
  label: Orchesty.io 3.0 API
  slug: 3.0-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orchesty/openapi/_ae-authored/orchesty-3.0-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orchesty.io
  spf: false
hosts:
- cert_expires: Dec 14 06:06:57 2026 GMT
  host: orchesty.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orchesty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orchesty.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Orchesty.io
provider_slug: orchesty
slug: orchesty-domain-security
source_filename: orchesty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orchesty.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 06:06:57 2026 GMT\n  hsts: false\ndomains:\n- domain: orchesty.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/orchesty/security/orchesty-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Integration
- Platform
- Automation
- Artificial Intelligence
- Open Source
---
