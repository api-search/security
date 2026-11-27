---
api_specs:
- filename: cyphrex-io-api-openapi.json
  format: json
  label: Cyphrex API API
  slug: cyphrex-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyphrex-io/openapi/_original/cyphrex-io-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cyphrex.io
  spf: true
hosts:
- cert_expires: Dec 18 06:32:22 2026 GMT
  host: cyphrex.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cyphrex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cyphrex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cyphrex
provider_slug: cyphrex-io
slug: cyphrex-io-domain-security
source_filename: cyphrex-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cyphrex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 06:32:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cyphrex.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cyphrex-io/security/cyphrex-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
